# Code at end of body
In this file you can be specify content that will be inserted at the end of the BODY-section.

```php
$code_at_end_of_body = "";
$code_at_end_of_body .= <<<EOT
    ...
EOT;
```

The content is specified between EOT and can be multiline.