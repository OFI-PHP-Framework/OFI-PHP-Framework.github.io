## OFI PHP Framework official documentation

##### Bahasa Indonesia
Kamu bisa mengunjungi github OFI PHP framework
disini : https://github.com/teguh02/ofi-php-framework

Apa itu OFI PHP Framework?
1. OFI PHP Framework adalah sebuah framework PHP yang mengadaptasi dari framework laravel dan codeigniter.
2. OFI PHP Framework adalah sebuah framework PHP yang di desain untuk kecepatan 

### Struktur folder
<br>

[![d6UTzJ.md.png](https://iili.io/d6UTzJ.md.png)](https://freeimage.host/i/d6UTzJ)

<br>
Penjelasan
1. App merupakan folder yang memuat file file controller, model middleware dan lain lain
2. assets merupakan folder yang memuat file css, js dan gambar 
3. route merupakan folder yang memuat aturan route framework
4. sql merupakan folder contoh sql yang siap import
5. vendor merupakan folder vendor/system OFI PHP Framework
6. Views merupakan folder yang memuat layout views (akan dibahas pada BAB views)
7. .gitignore merupakan file github
8. .htaccess merupakan file htaccess default Framework
9. composer merupakan file konfigurasi milik composer sendiri
10. config.php merupakan file yang berisi konfigurasi aplikasi
11. index.php merupakan file utama supaya Framework ini berjalan
12. readme.md merupakan file github

### Konfigurasi aplikasi

Supaya OFI PHP Framework berjalan dengan baik, kamu perlu mengkonfigurasikan file config.phpnya terlebih dahulu seperti ini contohnya.

```
<?php

/**
 * OFI PHP Framework
 * Define project name and environment settings.
 */

 // Your Project Name
define('PROJECTNAME', 'OFI Framework');

 // Your Project Environment production or development
define('ENVIRONMENT', 'development');

// Your Project URL
// do not use the '/' at the end of the url http: // localhost: 9000
define('PROJECTURL', 'http://localhost:9000');

// Upload file function limiter 
// default 1044070 = 1 mb
define('MAXUPLOAD', 1044070);


// Database MYSQLI connection configuration
$config = [
    'driver'        => 'mysql',
    'port'          => 3306,
    'host'          => 'localhost',
    'dbname'        => 'ofi',
    'username'      => 'root',
    'password'      => '',
    'timestamp'     => false // Give created_at and updated_at to your table
];


/**
 * Define SEO tag for your website
 * please change according to your needs.
 *
 * What is google-site-verification?
 * For example for the tag :
 * <meta name="google-site-verification" content="ZJTLoB1wuXx1aV_gw0ATcBmS0tk8M3IuUkOMi_Qi6C8" />
 *
 * You can only take the meta tag content, and then the content is
 *          ZJTLoB1wuXx1aV_gw0ATcBmS0tk8M3IuUkOMi_Qi6C8
 * please put thats content in define('GoogleSiteVerification', '');
 */

// Description for your website
define('DESCRIPTION', 'OFI PHP Framework');
define('AUTHOR', 'Teguh Rijanandi');

// Separate with comma
define('KEYWORDS', 'Framework, PHP, Backend');
define('GoogleSiteVerification', '');

/**
 * Define your sites mailer
 * This is default config for gmail
 * Default Mailer is use SMTP.
 *
 * Tips!
 * First you must turn on Access for less secure apps in
 * https://myaccount.google.com/lesssecureapps
 *
 * And then you can change this gmail username and password
 * with your's gmail account
 *
 * Enable SMTP debugging
 * 0 = off (for production use)
 * 1 = client messages
 * 2 = client and server messages
 */
define('SMTPSecure', 'tls');
define('Host', 'smtp.gmail.com');
define('Port', 587);
define('GmailUsername', 'youremail@gmail.com');
define('GmailPassword', 'yourpass');
define('SMTPDebug', 0);
define('senderEmail', 'system@ofiFramework.com');
define('senderName', 'OFI Framework Mailing System');

```

### Menjalankan pada development mode
1. Pertama masuk kedalam direktori framework, contohnya pada gambar dibawah ini
path nya adalah ``` C:\xampp_7.1\htdocs\OFI-PHP-FW ```
<br>

[![d6UTzJ.md.png](https://iili.io/d6UTzJ.md.png)](https://freeimage.host/i/d6UTzJ)

<br>

2. Kedua silahkan buka terminal atau cmd lalu masuk kedalam direktori sesuai path diatas selanjutnya ketik ```composer serve``` maka otomatis framework akan berjalan pada  http://localhost:9000/

<br>

[![d6U1bs.md.png](https://iili.io/d6U1bs.md.png)](https://freeimage.host/i/d6U1bs)

<br>

[![d6UGzG.md.png](https://iili.io/d6UGzG.md.png)](https://freeimage.host/i/d6UGzG)
