# Code at end of head
In this file you can be specify content that will be inserted at the end of the HEAD-section.

```php
$code_at_end_of_head = "";
$code_at_end_of_head .= <<<EOT
    ...
EOT;
```

The content is specified between EOT and can be multiline.