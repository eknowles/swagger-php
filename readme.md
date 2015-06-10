swagger-php
============

 - [![1.x Build Status](https://secure.travis-ci.org/zircote/swagger-php.png?branch=1.x)](http://travis-ci.org/zircote/swagger-php) `1.x branch`

Swagger-PHP is a PHP library that serves as an annotations toolkit to produce [Swagger Doc](http://swagger.wordnik.com)
it makes use of the [Doctrine Common library](http://www.doctrine-project.org/projects/common.html) for
annotations support.

To report issues or ask questions please feel free to submit to [Github Issues](https://github.com/zircote/swagger-php/issues)

Download / Installation
------------------------
 - pear: http://zircote.com/pear
 - [composer](http://getcomposer.org/): [zircote/swagger-php](https://packagist.org/packages/zircote/swagger-php)
 - tarball: https://github.com/zircote/swagger-php/downloads
 - Clone via git: https://github.com/zircote/swagger-php.git

Documentation
--------------
Documentation is available at http://zircote.com/swagger-php

 To submit changes, additions or updates to the documentation or swagger-php itself please fork the project and submit a pull request. Documentation resides within the `gh-pages` branch.

Features
-------------------
 - Fully compatible with the full swagger documented proposal.
 - Full project discovery
 - Standalone CLI phar implementation
 - Free

 More on Swagger:
  * http://swagger.io/
  * https://github.com/swagger-api/swagger-spec/
  * https://github.com/outeredge/SwaggerModule a ZF2 Module implementing swagger-php

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/zircote/swagger-php/trend.png)](https://bitdeli.com/free "Bitdeli Badge")


BBC Swagger
---

Use --external option to only output APIs that contain paths starting with 'external'.
Use --internal option to only output APIs that contain paths **not** starting with 'external'.

Example shell command

```
#!/bin/sh
mkdir ~/BBC/mdt-mobileapi/public/swagger-app-definition/external
cd ~/BBC/mdt-mobileapi/public/swagger-app-definition/external
php /Users/ed/PhpstormProjects/swagger-php/bin/swagger /Users/ed/BBC/mdt-mobileapi/application/MobileApi/ -o ~/BBC/mdt-mobileapi/public/swagger-app-definition/external --external


mkdir ~/BBC/mdt-mobileapi/public/swagger-app-definition/internal
cd ~/BBC/mdt-mobileapi/public/swagger-app-definition/internal
php /Users/ed/PhpstormProjects/swagger-php/bin/swagger /Users/ed/BBC/mdt-mobileapi/application/MobileApi/ -o ~/BBC/mdt-mobileapi/public/swagger-app-definition/internal --internal
```