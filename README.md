# Sublime Text

## 1. Modules - Packages
The awesome thing about sublime text is that it's super light-weight.
There are however a ton of modules created by other devs.

### 1.1 Package Control
This is **The** module. Consider it a **MUST**.
Having this will make installing other modules a breeze.

The installation process is fairly simple:

1. Go to ```Preferences > Browse Packages…```.
2. Browse up a folder and then into the ```Installed Packages``` folder.
3. Copy [Package Control.sublime-package](sublime-text/Package Control.sublime-package) here.
4. Restart sublime.

### 1.2 Module installation
After installing *Package Control* you can use it to install other plugins.

Package Control is driven by the *Command Palette*.
To open the palette, press ```ctrl+shift+p``` (Win, Linux) or ```cmd+shift+p``` (OS X).
All Package Control commands begin with Package Control:, so start by typing ```Package```.

### 1.3 MUST install modules
#### 1.3.1 Phpcs
*Write better quality and consistent code*  

1. Install code sniffer via composer: ```composer global require "squizlabs/php_codesniffer=*"```.
2. Install PHP Mess Detector via composer: ```composer global require --dev phpmd/phpmd```.
3. Add composer bin to path (if it's not already):

```
PATH=$PATH:~/.composer/vendor/bin/
export PATH
```
4. Install Phpcs with Package Control.
5. Add settings from *settings-phpcs* to ```Preferences > Package Settings > PHP Code Sniffer > Settings User```.

#### 1.3.2 Syntax support modules
1. Install the following with Package Control: Sass, Twig.

#### 1.3.3 SublimeCodeIntel
1. Install with Package Control.

#### 1.3.4 Xdebug Client
1. Install xdebug: ```sudo apt-get install php5-xdebug```.
2. Enable xdebug: ```sudo php5enmod xdebug```.
3. Add the contents of xdebug.ini to ```/etc/php5/mods-available/xdebug.ini```.
4. Install ```Xdebug Client``` with Package Control.
5. Copy the contents of settings-xdebug.json to ```Preferences > Package Settings > Xdebug > Settings User```.

*Keep in mind that these are general settings.*
*[Some will need to be changed per project](https://github.com/martomo/SublimeTextXdebug).*

### 1.4 SHOULD install modules
#### 1.4.1 Alignment
1. Install with Package Control.
2. Profit$$ (default: ctrl + alt + a).

#### 1.4.2 DocBlockr
1. Install with Package Control.
2. Adds a PHPDoc template before fields, functions, classes etc.
3. Usage: write ```/**``` and then hit enter.

## 2. General preferences
This are all-around settings that you **SHOULD** use to improve your sublime text experience.

### 2.1 Install
1. Fire up Sublime Text, and go to ```Preferences > Settings - User```.
   This will enable you to keep your settings, even if you update your installation at some point.
2. Copy & paste the contents of [settings-user.json](sublime-text/settings-user.json) and save the file.


## 3. Syntax - specific preferences
These are PHP specific settings that you **MUST** use to guide you into applying many of the conventions that we use.
They will only be applied to files that are mapped to this syntax (by default ```.php``` files).

### 3.1 Install

#### 3.1.1 PHP
1. Fire up Sublime Text, and open a random PHP(\*.php) file.
2. Go to ```Preferences > Settings - More > Syntax Specific - User```.
2. Copy & paste the contents of [settings-php.json](sublime-text/settings-php.json) and save the file.

#### 3.1.2 Javascript
1. Start Sublime Text and open any javascript(\*.js) file.
2. Go to ```Preferences > Settings - More > Syntax Specific - User```.
3. Copy & paste the contents of [settings-js.json](sublime-text/settings-js.json) and save the file.

#### 3.1.3 CSS/Sass
1. Start Sublime Text and open any css(\*.css) and sass(\*.scss) file.
2. Go to ```Preferences > Settings - More > Syntax Specific - User```.
3. Copy & paste the contents of [settings-css.json](sublime-text/settings-css.json) and save the file.

#### 3.1.4 HTML
1. Start Sublime Text and open any html(\*.html) file.
2. Go to ```Preferences > Settings - More > Syntax Specific - User```.
3. Copy & paste the contents of [settings-html.json](sublime-text/settings-html.json) and save the file.

#### 3.1.5 TWIG
1. Start Sublime Text and open any html(\*.html.twig) file.
2. Go to ```Preferences > Settings - More > Syntax Specific - User```.
3. Copy & paste the contents of [settings-html-twig.json](sublime-text/settings-html-twig.json) and save the file.

