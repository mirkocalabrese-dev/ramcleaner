# ramcleaner
Clean RAM from unused inodes, dentries and pagecache on Debian and OpenWrt

ramcleaner is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>

Name: ramcleaner

Version: 0.1

License: GPLv3

Author: Mirko Calabrese - mirkocalabrese.dev@gmail.com

Website: https://www.mirkocalabrese.eu

Creation Date: 2023-07-21

Last Update: 2023-07-21

Copyright 2023 Mirko Calabrese

Description: This tool cleans RAM from pagecache, dentries and unused inodes.
This tool runs from version 2.6.16 on the Linux kernel, drop_caches does not exist in earlier versions of that kernel.

This is the means of drop_caches's values:

1: it cleans pagecache

2: it cleans dentries and inodes

3: it cleans pagecache, dentries and inodes

## Tested on:
Debian 11
Debian 12
OpenWrt ATTITUDE ADJUSTMENT 12.09, r36088

## Dependences for Debian 11-12
```
# apt-get install git bash
```

## Dependences for OpenWrt ATTITUDE ADJUSTMENT 12.09, r36088
```
# opkg install bash git
```


## Installation
To install ramcleaner, type these commands:
```
$ git clone git://github.com/FreeNIX-Security-Labs/memcleaner/
$ cd ramcleaner
$ chmod 755 install.sh
# ./install.sh
```
