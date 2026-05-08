---
title: Usage
locale: en
status: stable
---

# Usage

```php
// Read back
$delta = json_decode($article->body, true);
$converter = new \Dskripchenko\LaravelAdminQuill\Converter\DeltaToHtml();
echo $converter->convert($delta);
```

Custom Quill toolbar:

```vue
<DskWysiwyg :toolbar="['bold', 'italic', { header: [1, 2, false] }, 'image']" />
```

