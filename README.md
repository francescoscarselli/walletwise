![Screen](https://raw.github.com/francescoscarselli/walletwise/master/web/images/favicon-32x32.png) WalletWise
=================================

WalletWise (New [Economizzer](http://www.economizzer.org)) is a simple and open-source personal finance manager system made in PHP <br />[Yii Framework 2](http://www.yiiframework.com).
<br />It is available in the following languages:  Italian, English, Spanish, Portuguese, Russian, Korean, Hungarian and French.

![Screen](https://raw.github.com/francescoscarselli/walletwise/master/web/images/screen.png)
<br />Learn more about the features by visiting the [Wiki](http://github.com/francescoscarselli/walletwise/wiki/)


Live Demo
------------
Unfortunately, we don't have a new demo site but there's the old one made by the original creator.
<br />You can try the old one demo site: [here](http://www.economizzer.org/web)
> Use the user "joe" and password "123456".
<br />We'll add more features in the future so that site will be out of date.
<br />Support us to buy a new demo domain. Thank you.


Requirements
------------
The minimum requirements that this application requires are: PHP>7.0 and apache2 or nginx.
> Required libraries: mysql, php, composer, libapache2-mod-php, php-mbstring, php-xml, php-curl


Installation
------------
~~~
sudo apt update && sudo apt upgrade -y
sudo apt install apache2 (or nginx) -y
sudo apt install curl php composer libapache2-mod-php php-mbstring php-xml php-curl mysql-server -y
git clone https://github.com/francescoscarselli/walletwise.git
cd walletwise
composer update && composer install
~~~
* You need to configure yourself MySQL and Apache2 for your domain. If you need help to setup everything, visit the [wiki page](http://github.com/francescoscarselli/walletwise/wiki/).


Configuration
-------------
In the folder **walletwise/config/db.php** set as your parameters:
```php
return [
    'class' => 'yii\db\Connection',
    'dsn' => 'mysql:host=127.0.0.1;dbname=walletwise',
    'username' => 'root',
    'password' => '<password/blank>',
    'charset' => 'utf8',
    'enableSchemaCache' => true,
];
```
Import the sql database file located in:
> inc/walletwise.sql

Check if everything is working by going to your **http://hostname.local/web**.
<br />**NOTE:** This path is only for who has the WalletWise folder in the root of the /var/www/html folder.
<br /> Use these **credentials** to log-in:
> User: "admin" and password: "123456"


Contribution
-------------
Please see [CONTRIBUTING](CONTRIBUTING.md).


License
-------------
Economizzer, rights © 2014 Gustavo G. Andrade.<br /> 
WalletWise, rights © 2023-2026 Deltwin [(Francesco Scarselli)](https://github.com/francescoscarselli).<br />
It is free software, and may be redistributed under the terms specified in the
[LICENSE](LICENSE.md) file.


Donations
-------------
To encourage the developer with new enhancements, buy a demo domain, or even to buy him a good beer, <br />support the project by making a [Donation](https://buymeacoffee.com/fraank).


Thanks to
-------------
[![Yii2](https://img.shields.io/badge/Powered_by-Yii_Framework-green.svg?style=flat)](http://www.yiiframework.com)
<br />[Gugoan](https://github.com/gugoan/economizzer)
