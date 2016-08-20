# Code at end of body
In der Datei '**code_at_end_of_body.php**' können Inhalte angegeben sein, die am Ende des BODY-Tags eingefügt werden.

Der Inhalt wird zwischen EOT angegeben und kann somit mehrzeilig vorliegen.

```php
$code_at_end_of_body = "";
$code_at_end_of_body .= <<<EOT
    ...
EOT;
```