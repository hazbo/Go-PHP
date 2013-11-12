# Go-PHP

Go-PHP is the start of a small framework that will allow
you to write PHP Extensions using [Go-Lang](http://golang.org/).
I have [written about this here](http://hazbo.github.io/2013/11/09/go-and-php/).

### Prerequisites

  - gcc
  - gccgo
  - make
  - php
  - phpize

General build tools. A `build-essentials` package may be needed.

### Building

	$ git clone https://github.com/hazbo/Go-PHP.git
	$ cd Go-PHP
	$ phpize
	$ ./configure
	$ sudo bash ./goconfigure
	$ make
	$ sudo make install

### Extras

Don't forget to add `extension=framework.so` to your `php.ini` file.
You may need to restart PHP e.g.

	$ sudo /etc/init.d/php5-fpm restart

If using the FPM handler.