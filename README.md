Documentation
UwAmp Install
Update PHP or Apache config manualy
MySQL Account
Macros

UwAmp Install
UwAmp is available in 3 formats, exe, rar et zip.

For Zip and Rar format, just uncompress.
The Exe is an NSIS installtion with LZMA compression.

To Remove UwAmp just remove the folder.

Update PHP or Apache config manualy
If you want change configuration directly in file update this files :

Config file for apache : bin/apache/conf/httpd_uwamp.conf
Config file for PHP : bin/php/php_[*]/php_uwamp.ini
Config file for MySQL : database/mysql-*/my_uwamp.ini


MySQL Account
utilisateur "root"
mot de passe "root"



Macros
UwAmp use a macro to create configuration file with good path. You can use macro in all file with "_uwamp" in name.

Macros list

{APACHEPATH}
Absolute path to Apache : UwAmp\apache

{DOCUMENTPATH}
Absolute path to UwAmp www : UwAmp\www

{PHPPATH}
Absolute path to selected PHP version : UwAmp\bin\php\php_[CURRENT VERSION]\

{PHPAPACHE2FILE}
Absolute path to PHP DLL : UwAmp\bin\php\CURRENT PHP IN UWAMP CONTROL\CURRENT apache2.dll

{PHPEXTPATH}
Absolute path to PHP extention folder : UwAmp\bin\php\php_[CURRENT VERSION]\ext

{PHPMODULENAME}
Current PHP module name for Apache

{MYSQLPATH}
Absolute path to MySQL : UwAmp\database\mysql-[CURRENT VERSION]

{MYSQLBINPATH}
Absolute path to MySQL bin : UwAmp\database\mysql-[CURRENT VERSION]\bin

{MYSQLDATAPATH}
Absolute path to MySQL data path : UwAmp\database\mysql-[CURRENT VERSION]\data

{ONLINE_MODE}
If UwAmp is on Online mode, your website is available for all.
{ONLINE_MODE} will be replaced by :
Order allow,deny
Allow from all

If UwAmp is on Offline mode, your website is available only for your computer.
{ONLINE_MODE} will be replaced by :
Order deny,allow
Allow from 127.0.0.1 localhost

[Download Here](https://www.uwamp.com/en/?page=download"Download")
