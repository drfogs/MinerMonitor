MinerMonitor
==============

This is a very basic monitor for your miners. With updated front end
(see [AUTHORS](AUTHORS) for a list of contributors)

#### Table of contents

* [Dependencies](#dependencies)
* [Download](#download)
* [Usage instructions](#usage-instructions)
* [TODOS](#todos)
* [Credits](#credits)
* [License](#license)

Dependencies
============
 * PHP enabled web server
 * fsock enabled for PHP
 * You can run a built in PHP server from your PC instead of a full server

Download
========
 * Git tree:   https://github.com/drfogs/minerMonitor
 * Clone with `git clone https://github.com/drfogs/MinerMonitor.git`

Usage instructions
==================
#### Updating from a previous version:
If updating from Derricke's version clear browsing data, otherwise it will throw a mixture of the previous version with this version.

#### On miner machines:
 * Run cpuminer with the command line option: `--api-bind 0.0.0.0:4048`
 * Open firewall incoming port tcp:4048

#### On Web Server
 * Download or clone repo
 * Modify minerHosts file with a list of your miners to monitor
 * Modify minerHosts path in config.ini
   * By default it will be in the same folder, but you can place it anywhere as long as you correctly set the path
 * Point web server to folder
 * Open firewall outgoing port tcp:4048

#### Simple built in php server
 * [Full Instructions](http://php.net/manual/en/features.commandline.webserver.php)
 * Install PHP for your OS
 * Go to the path where you cloned this repo
 * Run this command `php -S localhost:8000`
   * Terminal will show:
```
PHP Development Server started
Listening on localhost:8000
Document root is /var/www/public_html
Press Ctrl-C to quit
```

#### Finish
 * Point your browser to your webserver

TODOS
=====
 * [ ] Accurate total H/m to be implemented

Credits
=======
MinerMonitor is based on Birty's original version, forked from Derricke's fork
I fixed code formatting, remade some functions, added useability, etc.

License
=======
GPLv3.  See [LICENSE](LICENSE) for details.
