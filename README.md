This is a Composer-based installer for the [Lightning for Commerce](https://github.com/acquia/lightning-commerce) Drupal distribution.

## Get Started
```
$ composer create-project acquia/lightning-commerce-project MY_PROJECT
```
Composer will create a new directory called MY_PROJECT containing a ```docroot``` directory with a full Lightning for Commerce code base there. You can then install it like you would any other Drupal site.

## Source Control
If you peek at the ```.gitignore``` we provide, you'll see that certain directories, including all directories containing contributed projects, are excluded from source control. This might be a bit disconcerting if you're newly arrived from Planet Drush, but in a Composer-based project like this one, **you SHOULD NOT commit your installed dependencies to source control**.

When you set up the project, Composer will create a file called ```composer.lock```, which is a list of which dependencies were installed, and in which versions. **Commit ```composer.lock``` to source control!** Then, when your colleagues want to spin up their own copies of the project, all they'll have to do is run ```composer install```, which will install the correct versions of everything in ```composer.lock```.

## Copyright and license

   Acquia Lightning for Commerce Project
   
   Copyright (C) 2018 Acquia Inc.

   This program is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by    the Free Software Foundation; either version 2 of the License, or
   (at your option) any later version.

   This program is distributed in the hope that it will be useful,
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
   GNU General Public License for more details.

   You should have received a copy of the GNU General Public License along
   with this program; if not, write to the Free Software Foundation, Inc.,
   51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.

