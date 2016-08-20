# fe_conmunicator.html5
The file is the template for use in a page layout of the Contao CMS and located in the folder "/templates". About various settings can influence the behavior.

```php
<?php
//==================================================================================
// fe_conmunicator.html5
//----------------------------------------------------------------------------------
// Bringing two worlds together …
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
Path to the folder in which the Adobe MUSE exports will be found. The path may be modified as needed.

#dir
Path to the exported Adobe MUSE Site. Can be modified as needed.

#conf
| Parameter: | Werte: |Bedeutung: |
| -- | -- | -- |
| templateFile |[name.html]| Name of an Adobe-MUSE page that should be used for output. All page layouts that use this Contao template will then output the corresponding Adobe MUSE page. **If the value is "" or undefined, so the normal alias or file mapping takes place.**|
| stripComments |true/false| The specified HTML code is exempted from commentaries.<br>**Default = false**|
| useContaoJQuery |true/false| The used Adobe-MUSE version of jQuery is replaced by the version of Contao.<br>**If true, so replaceJQuery is ignored!**<br>**Default = false**|
| replaceJQuery |true/false| The used Adobe-MUSE version of jQuery is replaced with the version that ships with <.CONMUNICATOR>.<br>**Default = false**|
| centerPage |true/false| Center the hole page on screen. Useful for adaptive layouts<br>**Default = false**|

In general, the parameters can be deleted from the conf-array, then each enters the default behavior.