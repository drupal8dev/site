---
layout: post
title: Drupal\Core\Config\StorageException Failed to write configuration file
date: 2013-10-17 12:46
comments: true
categories: drupal8
---

Fix permissions for your files directory:

```
$ sudo chmod -R 777 sites/default/files
```
