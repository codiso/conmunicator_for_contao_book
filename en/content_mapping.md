# Content Mapping

To use this feature you can create device folders (desktop,tablet,phone) in the folder /conmunicator/devices/. Each device folder can contain a text file, which shall comply with the following notation.

```
content_mapping_[LANG].php
```

If a device has no specific file, the "desktop" version will be tried to load. If this file does not exist, the "content mapping" does not take place.

## XPath
Conmunicator uses the [DOMDocument](http://php.net/manual/de/class.domdocument.php "PHP-DOMDocument") from PHP to manipulate the DOM structure. In this file you can use the following objects:

| Object | Bedeutung |
|-|-|
|$doc|DThes [DOMDocument](http://php.net/manual/de/class.domdocument.php) used by Conmunicator|
|$xpd|The [XPath object](http://php.net/manual/de/class.domxpath.php) used by Conmunicator|
|$this|The Contao object for the page|

### Beispiel:

With an [XPath-Query](https://www.w3.org/TR/xpath/) you can select DOM-Elements. These Elements can then be manipulated by PHP.

```php
$query = '//nav[@id="menuu20128"]';
$nodes = $xpd->query($query);
foreach($nodes as $node) {
    $node->innerHTML = $this->main;
}
```