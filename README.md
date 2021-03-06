Z-Ray-Laravel
=============

Laravel 4 Extension for Zend Server Z-Ray

This is an extension to add functionality to the Zend Server Z-Ray. It will result 
in additional tab(s) to be presented in the browser.

Panels
=============
- Laravel
- Session
- Logged User Info
- Views
- Events
- Configuration Values (For security reason is not activated by default. To Activate, modify $visibleConfigurations on zray.php)


Installation
------------

Create a directory named as desired, and add the contents of this repo within.

Example: (assuming default install directory for Zend Server)

```
    /usr/local/zend/var/zray/extensions/{extension-name}/zray.php
    /usr/local/zend/var/zray/extensions/{extension-name}/logo.png
```

NOTE: While the filename zray.php is required, the file logo.png can be named whatever 
you desire and is specified from within the zray.php code as below.

```php
    $zrayMagento->getZRay()->setMetadata(array(
        'logo' => __DIR__ . DIRECTORY_SEPARATOR . 'logo.png',
    ));
```

