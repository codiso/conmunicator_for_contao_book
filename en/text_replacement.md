# Text replacement

In the file **text_replacement.php** own text replacements can be defined.

```php
replace_text($search,$replace,$regex=false)
```

| Parameter | Description |
| -- | -- |
| $search |Text der gesucht werden soll. Ist **$regex=true**, so wird $search als RegEx interpretiert.|
| $replace |Text der als Ersetzung dienen soll.|
| $regex |Wahl ob die Erstezung als str_replace (false) oder als preg_replace (true) ausgeführt wird.|

