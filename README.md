sagepay-sdk-php
===============

Sage Pay PHP SDK for server and direct integrations (based on the official Sage Pay SDK).

This repository takes the official Sage Pay V3 PHP SDK and turns it into a composer compatible include for use with modern frameworks. No code has been modified from the existing Sage Pay code so it allows you to build your own wrappers for your integration. This is not an official Sage Pay package.

Warning
-----------
I make no warranty whatsoever for use of this repository and the code within it. Please always check source code yourself especially when using third-party payment software. It is your responsibility to check for exploits, vulnerabilities in the source code if you are using it in any project. The code has not been modified by myself but this repository could potentially be compromised by a third-party, you should verify the code yourself if using it. The source code itself is mainly provided by Sage Pay themselves but I also make no warranty for their work. If you would like to use this repository in a commercial project it is recommended you download the official Sage Pay integration files from http://www.sagepay.co.uk/support/find-an-integration-document/direct-integration-documents and create your own wrappers using this repository as a guide.

Install Composer
----------------

Run this in your terminal to get the latest Composer version:

<code>curl -sS https://getcomposer.org/installer | php</code>
Or if you don't have curl:
<code>php -r "readfile('https://getcomposer.org/installer');" | php</code>

This installer script will simply check some php.ini settings, warn you if they are set incorrectly, and then download the latest composer.phar in the current directory.

Installation
------------

To install this library to your project it is recommended to use composer.

Run:

<code>composer require ammaar23/sagepay-sdk-php</code>

There is a composer archive at:

https://packagist.org/packages/ammaar23/sagepay-sdk-php

Usage
-----

The Official SagePay SDK does not currently use namespaces so to use the SDK you simply run commands such as:
<code>
$api = SagepayApiFactory::create(SAGEPAY_SERVER, $config);
$api->setBasket($basket);
</code>

There is a working demo if you download the official SagePay PHP SDK at: http://www.sagepay.co.uk/support/find-an-integration-document/server-integration-documents

Updates
-------

I couldn't find any versioning info for the SagePay PHP SDK so please check yourself if you think this archive may be out of date or better yet you can make a request to update this repository yourself!

Copyright
---------

The SDK belongs to SagePay and is their intellectual property. No license information is available but this is a publicly accessible source code. I do not intend any copyright infringement and am simply creating a wrapper to aid developers (including myself) to use the SagePay SDK in their composer compatible projects.

Contact
-------

If you need to contact me you can get in touch with me via my email: ammaarlatif_14@hotmail.co.uk
