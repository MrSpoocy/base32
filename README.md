base32
======

Base32 Encoder/Decoder for PHP according to [RFC 4648](https://tools.ietf.org/html/rfc4648).

[![Build Status](https://secure.travis-ci.org/ChristianRiesen/base32.png)](http://travis-ci.org/ChristianRiesen/base32)

[![Latest Stable Version](https://poser.pugx.org/christian-riesen/base32/v/stable.png)](https://packagist.org/packages/christian-riesen/base32) [![Total Downloads](https://poser.pugx.org/christian-riesen/base32/downloads.png)](https://packagist.org/packages/christian-riesen/base32) [![Latest Unstable Version](https://poser.pugx.org/christian-riesen/base32/v/unstable.png)](https://packagist.org/packages/christian-riesen/base32) [![License](https://poser.pugx.org/christian-riesen/base32/license.png)](https://packagist.org/packages/christian-riesen/base32)

Usage
-----

```php
<?php

// Include class or user autoloader
use Base32\Base32;

$string = 'fooba';

// $encoded contains now 'MZXW6YTB'
$encoded = Base32::encode($string);

// $decoded is again 'fooba'
$decoded = Base32::decode($encoded);
```

About
=====

Initially created to work with the [one time password project](https://github.com/ChristianRiesen/otp), yet it can stand alone just as well as [Jordi Boggiano](http://seld.be/) kindly pointed out. It's the only Base32 implementation that passes the test vectors and contains unit tests as well.

Goal
----
Have a RFC compliant Base32 encoder and decoder. The implementation could be improved, but for now, it does the job and has unit tests. Ideally, the class can be enhanced while the unit tests keep passing.

Requirements
------------

PHP 7.4+

Tests run on PHPUnit 9.5, with PHP 7.4 and later.

Author
------

Christian Riesen <chris.riesen@gmail.com> http://christianriesen.com

Acknowledgements
----------------

Base32 is mostly based on the work of https://github.com/NTICompass/PHP-Base32
