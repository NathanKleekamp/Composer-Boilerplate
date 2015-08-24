# Composer Boilerplate

A base `composer.json` file for Wordpress (installed in its [own directory](http://codex.wordpress.org/Giving_WordPress_Its_Own_Directory)) that treats WP, themes, and plugins as dependencies.

Uses [WPackagist](http://wpackagist.org/) for public plugins and themes, and `git` for privately hosted plugins, themes, and Wordpress.

Uses Fancyguy's [webroot-installer](https://github.com/fancyguy/webroot-installer) to install Wordpress core files in the proper directory.

Each privately hosted repo needs to have it's own `composer.json` file following the `composer.json` [schema](https://getcomposer.org/doc/04-schema.md).

Run the following to install the dependencies after cloning the repo containing the `composer.json` file.
```
$ composer install
```

Commit the `composer.lock` to your repo to make sure dependancies match across all machines.

`composer update` will update the dependancies after revving the version numbers in the `composer.json` file.

```
$ composer update
```
