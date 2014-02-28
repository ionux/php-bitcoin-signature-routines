PHP bitcoin signature routines

PHP routines for verifying Bitcoin signatures.  Requires PHP 5.3.2 and the extension GMP 4.2.0 or better. GMP may be available in a package called "php5-gmp" or similar for your system.


Pakages
-------
Ubuntu: http://packages.ubuntu.com/search?keywords=php5-gmp
Debian: https://packages.debian.org/search?keywords=php5-gmp
Red Hat: http://rpmfind.net/linux/rpm2html/search.php?query=gmp.so
CentOS (5.2): http://lists.centos.org/pipermail/centos/2010-November/101183.html
Slackware: http://search.slackware.eu/cgi-bin/package.cgi/inspect/slackware-14.0/slackware/l/gmp-5.0.5-i486-1.txz
Source: https://gmplib.org/#DOWNLOAD


Usage
-----
The main code is in verifymessage.php, with tests in test/verifymessage.php.  You will probably want to encapsulate the code more nicely, but since the ECC library needs to be configured specially and I am not up-to-date on the latest PHP packaging hotness anyway, I figured it would be best to leave that up to users to do how they like best.
