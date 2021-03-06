#fe_conmunicator.html5
Die Datei ist das Template für die Nutzung in einem Seitenlayout des Contao-CMS und befindet sich im Ordner "/templates". Über verschiedene Einstellungen lässt sich das Verhalten beeinflussen.

```php
<?php
//==================================================================================
// fe_conmunicator.html5
//----------------------------------------------------------------------------------
// Conmunicator. – Integrating Adobe Muse CC with a CMS
//==================================================================================
session_start();

$cmu["themePath"] 	= "conmunicator/export/";
$cmu["dir"] 		= $cmu["themePath"]."muse/";
$cmu["conf"] 		= array(
							"templateFile" => "",
							"stripComments" => true,
							"useContaoJQuery" => false,
							"replaceJQuery"	=> false,
                            "centerPage" => false,
						);

include("conmunicator/core/conmunicator.php");
?>
```
#themePath
Pfad auf den Ordner in dem die Adobe Muse CC Exporte zu finden sein werden. Der Pfad kann bei Bedarf abgeändert werden.

#dir
Pfad auf die exportierte Adobe Muse CC Site. Kann bei Bedarf abgeändert werden.

#conf
| Parameter: | Werte: |Bedeutung: |
| -- | -- | -- |
| templateFile |[name.html]| Name einer Adobe MUSE Seite, die zur Ausgabe genutzt werden soll. Alle Seitenlayouts die dieses Contao-Template nutzen, werden dann mit der korrespondierenden Adobe Muse CC Seite ausgegeben. **Ist der Wert "" oder undefiniert, so tritt das normale Alias- oder File-Mapping in Kraft.**|
| stripComments |true/false| Der ausgegebene HTML-Code wird von Kommentaren befreit.<br>**Default = false**|
| useContaoJQuery |true/false| Die von Adobe MUSE genutzte Version von jQuery wird durch die Version von Contao ersetzt.<br>**Ist dieser Wert true, so wird replaceJQuery ignoriert!**<br>**Default = false**|
| replaceJQuery |true/false| Die von Adobe MUSE genutzte Version von jQuery wird durch die Version ersetzt, die mit <.CONMUNICATOR> ausgeliefert wird.<br>**Default = false**|
| centerPage |true/false| Zentrieren der Site auf dem Bildschirm. Nützlich für adaptive Layouts.<br>**Default = false**|

Generell können die Parameter aus dem conf-Array gelöscht werden, dann tritt jeweils das Standardverhalten ein.
