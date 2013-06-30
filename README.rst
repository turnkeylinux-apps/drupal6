Drupal 6 - Content Management Framework
=======================================

`Drupal`_ is an open source content management platform licensed under
the GPL. Equipped with a powerful blend of features, Drupal can support
a variety of websites ranging from personal blogs, corporate brochures
and large community-driven websites.

This is the previous stable version of Drupal. The current latest stable
version of Drupal is `Drupal 7`_.

This appliance includes all the standard features in `TurnKey Core`_,
and on top of that:

- Drupal configurations:
   
   - Installed from package management. See /var/www for links to file
     paths
   - Search engine friendly out of the box
   - TKLBAM configured to skip cache and sessions database tables
     (smaller backups)

- Bundled Drupal modules (installed to
  /var/www/config/sites/all/modules):
   
   - `Views`_: A smart query builder for controlling how Drupal content
     is presented.
   - `CCK`_: Content Creation Kit - a powerful toolkit for creating
     custom content types.
   - `Panels`_: Drag and drop customized layouts for pages, nodes and
     blocks.
   - `Backup and migrate`_: Backup and restore your Drupal site
     on-demand or on a schedule.
   - `Devel`_: A suite of helper modules for Drupal module and theme
     developers.
   - `Drush`_: a command line shell and Unix scripting interface for
     Drupal.
   - `CKEditor`_: Enables CKeditor (a WYSIWYG editor) instead of plain
     text fields.``_
   - `IMCE`_: Powerful image file uploader and browser, with support for
     on the fly resizing.
   - `CAPTCHA`_: Thwart spammers by adding image or text based CAPTCHAs
     to your site.
   - `PathAuto`_: Auto-generate search engine friendly URLs (SEO).
   - `GlobalRedirect`_: Alias 301 redirects, prevents duplicate content.
     (SEO)``_
   - `FiveStar`_: Simple five-star voting widget for nodes.
   - `ImageCache`_: Setup presets that performs automatic image
     processing.
   - `Webform`_: Create forms and questionnaires.``_
   - `Logintoboggan`_: Improves Drupal's login system.
   - `Admin\_menu`_: Adds dropdown administration menu to the top of the
     screen.
   - `Tagadelic`_: Makes weighted tag clouds from your taxonomy terms.
   - `Lightbox2`_: Places images above your current page, not within.
   - `ModuleInfo`_: Adds essential information to the admin modules
     page.``_
   - `Google analytics`_: Adds Google Analytics js tracking code to all
     your site's pages.

- SSL support out of the box.
- `PHPMyAdmin`_ administration frontend for MySQL (listening on port
  12322 - uses SSL).
- Postfix MTA (bound to localhost) to allow sending of email (e.g.,
  password recovery, user registration).
- Webmin modules for configuring Apache2, PHP and MySQL.

Note: Drupal 6 includes a built-in *update status module*.

- When enabled could produce confusing/annoying version notifications.
- This is due to drupal6 being installed and updated via the APT package
  manager, instead of manually from the upstream source code.

Known issues
------------

- The Drupal 6 installation will fail if `client-side scripting is
  disabled`_.

Credentials *(passwords set at first boot)*
-------------------------------------------

-  Webmin, SSH, MySQL, phpMyAdmin: username **root**

.. _Drupal: http://drupal.org/
.. _Drupal 7: http://www.turnkeylinux.org/drupal7
.. _TurnKey Core: http://www.turnkeylinux.org/core
.. _Views: http://drupal.org/project/views
.. _CCK: http://drupal.org/project/cck
.. _Panels: http://drupal.org/project/panels
.. _Backup and migrate: http://drupal.org/project/backup_migrate
.. _Devel: http://drupal.org/project/devel
.. _Drush: http://drush.ws
.. _CKEditor: http://drupal.org/project/ckeditor
.. _IMCE: http://drupal.org/project/imce
.. _CAPTCHA: http://drupal.org/project/captcha
.. _PathAuto: http://drupal.org/project/pathauto
.. _GlobalRedirect: http://drupal.org/project/globalredirect
.. _FiveStar: http://drupal.org/project/fivestar
.. _ImageCache: http://drupal.org/project/imagecache
.. _Webform: http://drupal.org/project/webform
.. _Google analytics: http://drupal.org/project/google_analytics
.. _Logintoboggan: http://drupal.org/project/logintoboggan
.. _Admin\_menu: http://drupal.org/project/admin_menu
.. _Tagadelic: http://drupal.org/project/tagadelic
.. _Lightbox2: http://drupal.org/project/lightbox2
.. _ModuleInfo: http://drupal.org/project/moduleinfo
.. _backup and migrate: http://drupal.org/project/backup_migrate
.. _PHPMyAdmin: http://www.phpmyadmin.net/
.. _client-side scripting is disabled: http://www.turnkeylinux.org/forum/support/20090405/drupal-6-cd-boot-not-working
