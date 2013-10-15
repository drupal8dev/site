---
layout: post
title: "Installing Drupal 8"
date: 2013-10-15 01:20
comments: true
categories: drupal8 installation
---

{% img center /images/drupal8-setup-screen.png 700 380 'Drupal 8 Installation' 'Drupal 8 Installation' %}

## Getting Drupal 8

Drupal 8 is still pretty much in development, so there is no release on drupal.org yet. The best way to get the latest Drupal 8 is via git.

    git clone --branch 8.x http://git.drupal.org/project/drupal.git drupal8

### Notes 

1. Drupal 8 requires PHP 5.3. You'll need to set this up. More info [here](http://www.php.net/manual/en/install.php).
2. Drush 6 is not going to work with Drupal 8. We'll need the use the development version Drush 7. See https://github.com/drush-ops/drush#drush-versions.

## Installation

Once you've cloned the Drupal code, set up your files (sites/default/files) directory and copy default.settings.php to settings.php. Next point your browser to your Drupal 8 codebase.

Drupal 8 installation is very similar to Drupal 7, so nothing too difficult here. Note the awesome new theme.

### Drupal is installed. What's different here?

Here are a few things to note:

1. The following modules are now in core and enabled by default (using the standard profile)
   * _views_
   * _ckeditor:_ The WYSIWYG editor for Drupal 8
   * _tour:_ Provides guided tours.
   * _entity_reference:_ Provides field for referencing other entities
   * And yes, _toolbar_ and _overlay_ are still around.
2. Unlike Drupal 7, you're not logged in as administrator/user 1 after setup.
3. Bartik is now responsive.
4. Contact is now enabled in the standard profile and now accessible to anonymous users by default. Good.
