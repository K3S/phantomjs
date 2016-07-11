# [PhantomJS](http://phantomjs.org) - Scriptable Headless WebKit

PhantomJS ([phantomjs.org](http://phantomjs.org)) is a headless WebKit scriptable with JavaScript.  The latest [stable release](http://phantomjs.org/release-2.1.html) is version 2.1.

**Note**: Please **do not** create a GitHub pull request **without** reading the [Contribution Guide](https://github.com/ariya/phantomjs/blob/master/CONTRIBUTING.md) first. Failure to do so may result in the rejection of the pull request.

## Use Cases

- **Headless web testing**. Lightning-fast testing without the browser is now possible!
- **Page automation**. [Access and manipulate](http://phantomjs.org/page-automation.html) web pages with the standard DOM API, or with usual libraries like jQuery.
- **Screen capture**. Programmatically [capture web contents](http://phantomjs.org/screen-capture.html), including CSS, SVG and Canvas. Build server-side web graphics apps, from a screenshot service to a vector chart rasterizer.
- **Network monitoring**. Automate performance analysis, track [page loading](http://phantomjs.org/network-monitoring.html) and export as standard HAR format.

## Features

- **Multiplatform**, available on major operating systems: Windows, Mac OS X, Linux, and other Unices.
- **Fast and native implementation** of web standards: DOM, CSS, JavaScript, Canvas, and SVG. No emulation!
- **Pure headless (no X11) on Linux**, ideal for continuous integration systems. Also runs on Amazon EC2, Heroku, and Iron.io.
- **Easy to install**: [Download](http://phantomjs.org/download.html), unpack, and start having fun in just 5 minutes.

## Questions?

- Explore the complete [documentation](http://phantomjs.org/documentation/).
- Read tons of [user articles](http://phantomjs.org/buzz.html) on using PhantomJS.
- Join the [mailing-list](http://groups.google.com/group/phantomjs) and discuss with other PhantomJS fans.

PhantomJS is free software/open source, and is distributed under the [BSD license](http://opensource.org/licenses/BSD-3-Clause). It contains third-party code, see the included `third-party.txt` file for the license information on third-party code.

PhantomJS is created and maintained by [Ariya Hidayat](http://ariya.ofilabs.com/about) (Twitter: [@ariyahidayat](http://twitter.com/ariyahidayat)), with the help of [many contributors](https://github.com/ariya/phantomjs/contributors). Follow the official Twitter stream [@PhantomJS](http://twitter.com/PhantomJS) to get the frequent development updates.

## Build Steps

**Hardware requirements**

- RAM: at least 4 GB.
- Disk space: at least 3 GB.
- CPU: 1.8 GHz, 4 cores or more.

PhantomJS is still a web browser, albeit headless. Thus, building it from source takes a long time (mainly due to thousands of files in the WebKit module). Estimated build time for a 4-core system is 30 minutes.

**Linux requirements**

First, install the development packages of the following tools and libraries: GNU C++ compiler, bison, flex, gperf, Perl, Ruby, SQLite, FreeType, Fontconfig, OpenSSL, and ICU. The actual package names may vary from one distribution to another.

**On Debian-based distro (tested on Ubuntu 14.04 and Debian 7.0), run:**

sudo apt-get install build-essential g++ flex bison gperf ruby perl 
  libsqlite3-dev libfontconfig1-dev libicu-dev libfreetype6 libssl-dev 
  libpng-dev libjpeg-dev python libx11-dev libxext-dev

Note: It is recommend also to install ttf-mscorefonts-installer package.


**On Fedora-based distro (tested on CentOS 6), run:**

sudo yum -y install gcc gcc-c++ make flex bison gperf ruby 
  openssl-devel freetype-devel fontconfig-devel libicu-devel sqlite-devel 
  libpng-devel libjpeg-devel
