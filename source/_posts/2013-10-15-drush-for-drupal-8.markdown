---
layout: post
title: "Drush for Drupal 8"
date: 2013-10-15 02:02
comments: true
categories: drupal8, drush
---

Drush 6, the current stable version, does not work with Drupal 8. We will need Drush 7 for that. See https://github.com/drush-ops/drush#drush-versions.

Drush 7 is not stable yet so we want to keep running Drush 6 for Drupal 7 but use Drush 7 with Drupal 8. Here's how you can run multiple versions of Drush:

##### Step 1
Get Drush 7 via git. You could clone it to your home directory.
```
$ git clone https://github.com/drush-ops/drush.git ~/drush7
```

##### Step 2
Setup a bash alias by adding the following line to `~/.bash_profile` or `~/.bashrc`.
```
$ alias drush7='~/drush7/drush'
```

##### Step 3
Reload `~/.bash_profile` or `~/.bashrc`.
```
$ source ~/.bash_profile
```

##### Test
You should now be able to run Drush commands for drupal 8. Try clearing the cache with:
```
$ drush7 cc all
```

