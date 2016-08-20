# Text replacement
Bevor die Seite vom CMS ausgegeben wird ist hier die letzte Möglichkeit Textersetzungen durchzuführen. 

```php
$replacements[] = array(
	"search" => array(),
	"replace" => array(),
	["regex" => false,]
);
```

* preg_replace
* str_replace
