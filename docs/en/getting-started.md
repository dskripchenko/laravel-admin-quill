---
title: Getting Started
locale: en
status: stable
---

# Getting Started

`dskripchenko/laravel-admin-quill` is a sister-pack of `dskripchenko/laravel-admin`.
Install once — it auto-registers and surfaces in your admin.

## Install

```bash
composer require dskripchenko/laravel-admin-quill
php artisan migrate
```

## Configure

```bash
php artisan vendor:publish --tag=quill-config
```

Edit `config/quill.php`.


## What it adds

`@dskripchenko/laravel-admin-quill` exposes a `QuillField` for the
`Wysiwyg` slot.

```js
// resources/js/admin.js
import { QuillField } from '@dskripchenko/laravel-admin-quill'
import { registerField } from '@dskripchenko/laravel-admin'
import 'quill/dist/quill.snow.css'

registerField('wysiwyg', QuillField)
```

Output mode (html / delta):

```php
Wysiwyg::make('body')->mode('delta');
```

Stores Quill Delta JSON when `mode = delta`.

## See also

- [Usage](usage.md)
- [Glossary](https://github.com/dskripchenko/laravel-admin/blob/main/docs/en/glossary.md)
