# Base

This template extends no other template and has a `<!DOCTYPE html>`.


## How to extend ?

```twig
{% extends "@CVSymfonyTwigTemplates/base.html.twig" %}

{# Your code here #}
```

See also [Usage](../../README.md#Usage) for the Symfony configuration.


## Blocks

- **head** : is inside the `<head>`, it contains every other blocks and variables except the `{% block body %}`;
- **favicon** : is inside the `{% block head %}` and is empty;
- **stylesheets** : is inside the `{% block head %}` and is empty;
- **javascripts** : is inside the `{% block head %}` and is empty;
- **body** : is inside the `<body>` and is empty.


## Variables

Those HTML tags are rendered *only if* you define the corresponding variable in your template :
- **charset** : `<meta charset="{{ charset }}" />`;
- **viewport** : `<meta name="viewport" content="{{ viewport }}" />`;
- **baseUrl** : `<base href="{{ baseUrl }}" />`;
- **htmlHeadTitle** : `<title>{{ htmlHeadTitle }}</title>`;
- **metaDescription** : `<meta name="description" content="{{ metaDescription }}" />`;
- **canonical** : `<link rel="canonical" href="{{ canonical }}" />`.

This is always rendered :
- **app.request.locale** : `<html lang="{{ app.request.locale }}">`, defined in Symfony configuration.
