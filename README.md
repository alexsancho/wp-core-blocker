# WP Plugin: WP Core Blocker

## Installation
Preferred installation way is with composer:
```
$ composer require alexsancho/wp-core-blocker
```

## About
This plugin is meant for composer driven sites. It helps you to force installing/updating stuff only through composer or cli. It also blocks WordPress core from connecting to wp.org servers to make site faster and not to fail under local development with poor internet connection.

## Current Actions
* disables installing plugins and themes
* disables admin dashboard WP news widget
* disables all WP update checks for core, translations, themes, and plugins
* `define('WP_CORE_BLOCKER_DISABLE_GRAVATAR',true)` replaces all instances of Gravatar with a local image to remove external call

## Roadmap
* Disable all connections which cause errors without internet connections so that we can use whoops in local development without annoying errors.
