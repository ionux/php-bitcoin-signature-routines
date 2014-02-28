PHP bitcoin signature routines
-------------------------------
This is a collection of PHP routines for verifying Bitcoin signatures.  It requires PHP 5.3.2 and the extension GMP 4.2.0 or better. GMP may be available in a package called "php5-gmp" or similar for your system (see the Packages section below) or can be compiled from source and PHP configured with the --with-gmp option, if it's not already configured for it. The main class code is in class.phpBitcoinSignature.php with tests for the initial non-class code in test/verifymessage.php.  


Pakages
-------
Ubuntu: http://packages.ubuntu.com/search?keywords=php5-gmp<br />
Debian: https://packages.debian.org/search?keywords=php5-gmp<br />
Red Hat: http://rpmfind.net/linux/rpm2html/search.php?query=gmp.so<br />
CentOS (5.2): http://lists.centos.org/pipermail/centos/2010-November/101183.html<br />
Slackware: http://search.slackware.eu/cgi-bin/package.cgi/inspect/slackware-14.0/slackware/l/gmp-5.0.5-i486-1.txz<br />
Source: https://gmplib.org/#DOWNLOAD<br />

Other libraries may be required, so consult the official GMP documentation if you have questions regarding dependencies.


Usage
-----
Create an instance of the phpBitcoinSignature object and call the isMessageSignatureValid($address, $signature, $message) function with the required parameters.


Version
-------
- Initial release in 2013 by Joey Hewitt.
- Repository forked on 2/27/2014 from https://github.com/scintill/php-bitcoin-signature-routines
- Updated on 2/28/2014 by Rich Morgan to improve documentation, encapsulate code & add exception handling
