## OFI PHP Framework official documentation

##### Bahasa Indonesia
Kamu bisa mengunjungi github OFI PHP framework
disini : https://github.com/teguh02/ofi-php-framework

Apa itu OFI PHP Framework?
1. OFI PHP Framework adalah sebuah framework PHP yang mengadaptasi dari framework laravel dan codeigniter.
2. OFI PHP Framework adalah sebuah framework PHP yang di desain untuk kecepatan 

Struktur folder
[![d6UTzJ.md.png](https://iili.io/d6UTzJ.md.png)](https://freeimage.host/i/d6UTzJ)

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

### Konfigurasi

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

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/OFI-PHP-Framework/OFI-PHP-Framework.github-io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
