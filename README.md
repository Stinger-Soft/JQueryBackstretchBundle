# JQueryBackstretchBundle
jquery-backstretch Bundle for Symfony2

## Current Version

jquery-backstretch v2.0.4 - http://srobbin.com/jquery-plugins/backstretch/

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "stinger/jquery-backstretch-bundle": "~2.0.4"
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
        new Stinger\JQueryBackstretchBundle\StingerJQueryBackstretchBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update stinger/jquery-backstretch-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

### Usage

Add the css and js file where needed:

``` html
{% javascripts
	'bundles/stingerjquerybackstretch/js/jquery.backstretch.min.js'
%}
	<script src="{{ asset_url }}" ></script>
{% endjavascripts %}
```


# Licenses

Refer to the source code of the included files for license information

# References

1. http://srobbin.com/jquery-plugins/backstretch/
2. http://symfony.com

