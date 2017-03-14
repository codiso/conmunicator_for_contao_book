# Content Mapping

Um diese Funktion zu nutzen, können unter dem Ordner /conmunicator/devices/ Unterordner (desktop,tablet,phone) angelegt werden. In den Ordnern kann dann die entsprechende Textdatei angelegt werden.

```
content_mapping.php
```

Sollte für ein Endgerät keine spezifische Datei vorhanden sein, so wird automatisch auf "desktop" zurückgeschaltet. Sollte auch hier keine Datei vorhanden sein, findet das "Content Mapping" nicht statt.

## Funktionalitäten

Conmunicator nutzt das [DOMDocument](http://php.net/manual/de/class.domdocument.php "PHP-DOMDocument") aus PHP um DOM-Manipulationen durchzuführen. In der Datei kann auf drei Objekte zugegriffen werden:

| Variable | Bedeutung |
|-|-|
|$doc|Das [DOMDocument](http://php.net/manual/de/class.domdocument.php) des Conmunicator|
|$xpd|Das [XPath-Objekt](http://php.net/manual/de/class.domxpath.php) dex Conmunicator|
|$this|Das Contao-Objekt für die Seite|

### Beispiel:
Über einen [XPath-Query](https://www.w3.org/TR/xpath/) kann auf bestimmte Elemente in der DOM-Struktur eine Selektion erfolgen. Die Elemente können danach über PHP manipuliert werden.
 
```php
$query = '//nav[@id="menuu20128"]';
$nodes = $xpd->query($query);
foreach($nodes as $node) {
    $node->innerHTML = $this->main;
}
```



