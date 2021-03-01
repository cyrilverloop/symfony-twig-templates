# symfony-twig-templates

Twig templates for Symfony.

[![License](https://img.shields.io/github/license/cyrilverloop/symfony-twig-templates)](https://github.com/cyrilverloop/symfony-twig-templates/blob/trunk/LICENSE)


## Installation

### As a Composer depedency

In your project directory run
```shellsession
user@host project$ composer require "cyril-verloop/symfony-twig-templates"
```

### For development purposes

```shellsession
user@host ~$ cd [PATH_WHERE_TO_PUT_THE_PROJECT] # E.g. ~/projects/
user@host projects$ git clone https://github.com/cyrilverloop/symfony-twig-templates.git
user@host projects$ cd symfony-twig-templates
```


## Usage

The templates just needs to be referenced in the `config/packages/twig.yaml` file :

```yaml
twig:
    paths:
        '%kernel.project_dir%/vendor/cyril-verloop/symfony-twig-templates/templates': CVSymfonyTwigTemplates
```
You can also look at the `config/packages/twig.yaml` file of this project.

Then, you can inherit the templates :

```twig
{% extends "@CVSymfonyTwigTemplates/base.html.twig" %}
{# or #}
{% extends "@CVSymfonyTwigTemplates/layout.html.twig" %}

{# Your code here #}
```

The documentation of each template can be found in `resources/documentations/` :
- [base](resources/documentations/base.md)
- [layout](resources/documentations/layout.md)
