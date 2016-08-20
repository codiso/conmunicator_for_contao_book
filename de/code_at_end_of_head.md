# Code at end of head

In der Datei '**code_at_end_of_head.php**' können Inhalte angegeben sein, die am Ende des HEAD-Tags eingefügt werden.

Der Inhalt wird zwischen EOT angegeben und kann somit mehrzeilig vorliegen.

```php
$code_at_end_of_head = "";
$code_at_end_of_head .= <<<EOT
    ...
EOT;
```