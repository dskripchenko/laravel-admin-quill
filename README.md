> ## ⚠️ Пакет закрыт 17.08.2026
>
> Пакет был пустой обёрткой в 51 строку: только регистрация плагина. Vue-компонент редактора живёт в ядре, подключается парой строк в admin.js.
>
> Ставить его больше не нужно: всё, ради чего он заводился, есть в
> `dskripchenko/laravel-admin`. Установленным он не вредит, но и не добавляет
> ничего — кроме случая с поиском, где он ЗАМЕЩАЛ ядерный маршрут.

# dskripchenko/laravel-admin-quill

> 🌐 **English** · [Русский](docs/ru/README.md) · [Deutsch](docs/de/README.md) · [中文](docs/zh/README.md)

Alternative WYSIWYG engine on top of Quill (BSD-3-Clause). Outputs html and delta. Drop-in replacement for the default WYSIWYG field.

A sister-pack for [`dskripchenko/laravel-admin`](https://github.com/dskripchenko/laravel-admin).

[![Packagist](https://img.shields.io/packagist/v/dskripchenko/laravel-admin-quill)](https://packagist.org/packages/dskripchenko/laravel-admin-quill)
[![License](https://img.shields.io/packagist/l/dskripchenko/laravel-admin-quill)](LICENSE)

## Install

```bash
composer require dskripchenko/laravel-admin-quill
php artisan migrate
```

The plugin auto-registers via Laravel package discovery. To publish the
config:

```bash
php artisan vendor:publish --tag=quill-config
```

## Documentation

- [Getting started](docs/en/getting-started.md)
- [Usage](docs/en/usage.md)

## License

[MIT](LICENSE) © Denis Skripchenko
