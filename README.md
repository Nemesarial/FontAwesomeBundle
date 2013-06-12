NemFontAwesomeBundle - Font Awesome for Symfony2
===============================================

### Current Version

**Font Awesome 3.1.1** - Created & Maintained by Dave Gandy

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "nemesarial/fontawesome-bundle": "*"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Nemesarial\FontAwesomeBundle\QlFontAwesomeBundle(),
        // ...
    );
}
```

### Download the bundle using Composer and Install assets

``` bash
$ php composer.phar update nemesarial/fontawesome-bundle
$ php app/console assets:install --symlink web
```
Use the ``--symlink`` attribute to create links rather than copies of the resources

## Usage

### Easy Bootstrap + Font Awesome Integration

``head`` section in your template, e.g.

``` html
<link rel="stylesheet" type="text/css" href="{{ asset('..Your/Bootstrap/css..') }}" />
<link rel="stylesheet" type="text/css" href="{{ asset('bundles/qlfontawesome/css/font-awesome.min.css') }}" />
```

### Custom Bootstrap + Font Awesome Integration using LESS

[more information here](http://fortawesome.github.com/Font-Awesome/#integration)


# References

* [Font Awesome](http://fortawesome.github.com/Font-Awesome/)
* [Bootstrap](http://twitter.github.com/bootstrap/)
* [Symfony](http://symfony.com/)
