# symfony-twig-templates

A base Twig template for Symfony.

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

The template just needs to be referenced in the `config/packages/twig.yaml` file :

```yaml
twig:
    paths:
        '%kernel.project_dir%/vendor/cyril-verloop/symfony-twig-templates/templates': CVSymfonyTwigTemplates
```
You can also look at the `config/packages/twig.yaml` file of this project.

Then, your layout can inherit the base template :

```twig
{% extends "@CVSymfonyTwigTemplates/base.html.twig" %}

{# You code here #}
```
