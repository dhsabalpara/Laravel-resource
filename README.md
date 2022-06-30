
# Laravel Resources

## 🔗 Packages

 - [Laravel Socialite](https://laravel.com/docs/9.x/socialite)
    - [Laravel Socialite Example](https://techvblogs.com/blog/social-login-laravel-socialite)
 - [Laravel Cashier (Stripe)](https://laravel.com/docs/9.x/billing)
 - [Laravel Debugbar](https://packagist.org/packages/barryvdh/laravel-debugbar)
 - [Laravel Avatar](https://github.com/laravolt/avatar)
 - [Laravel Enum](https://laravel-news.com/laravel-enum-package-for-generating-enum-php-classes)
 - [Laravel Localization](https://github.com/spatie/laravel-translation-loader)
    - [Laravel Multi Language](https://dev.to/fadilxcoder/adding-multi-language-functionality-in-a-website-developed-in-laravel-4ech)
 - [Laravel Excel](https://docs.laravel-excel.com/3.1/getting-started/)
 - [Laravel Multiple Authentication](https://www.nicesnippets.com/blog/laravel-9-multiple-authentication-using-middleware)
 - [CRUD with Image Upload](https://docs.laravel-excel.com/3.1/getting-started/)
 - [Laravel Passport](https://blog.logrocket.com/laravel-passport-a-tutorial-and-example-build/)
 - [Laravel Sanctum](https://www.twilio.com/blog/build-restful-api-php-laravel-sanctum)
 - [Laravel Firebase](https://appdividend.com/2022/02/01/laravel-firebase-tutorial/)
 - [Laravel Dojah (Send OTP)](https://api-docs.dojah.io/reference/send-otp-1)
 - [Video API (Vonage)](https://www.vonage.com/communications-apis/video/features/)
 - [Covid-19 API](https://api.covid19api.com/country/india?from=2021-07-01T00:00:00Z&to=2021-08-01T00:00:00Z)

 ## Laravel Best Packages

- [Laravel Service-Repository Pattern](https://dev.to/saf1/implement-crud-with-laravel-service-repository-pattern-1dkl)
- [Laravel Permission](https://spatie.be/docs/laravel-permission/v5/introduction)
- [Laravel Best Practices](https://github.com/daxitzadafiya/laravel-best-practices)
- [Laravel RoadMap](https://github.com/LaravelDaily/Laravel-Roadmap-Learning-Path)

 # Popular 🔗 Links

 - [CronTab](https://crontab.guru/)
 - [Setup Virtual Host](https://ourcodeworld.com/articles/read/302/how-to-setup-a-virtual-host-locally-with-xampp-in-ubuntu)
 - [Install PHP On Ubuntu](https://tecadmin.net/install-php-ubuntu-20-04/)
 - [Install AnyDesk](https://computingforgeeks.com/how-to-install-anydesk-on-ubuntu/)
 - [Install TeamViewer](https://tecadmin.net/install-teamviewer-on-linux/)
 - [Install XAMPP](https://vitux.com/ubuntu-xampp/)
 - [Create API Documentation On Postman](https://www.softwaretestinghelp.com/postman-api-documentation/)
 - [Install Composer](https://linuxize.com/post/how-to-install-and-use-composer-on-ubuntu-18-04/)

## Connect Mysql Using Cli

Import Using Cli => sudo /opt/lampp/bin/mysql -u root -p db_name < db.sql

Export Using Cli => sudo /opt/lampp/bin/mysql -u root -p db_name > db.sql

## Start/Stop apache2 service

sudo service apache2 start

sudo service apache2 stop

## Start/Stop mysql service

sudo service mysql start

sudo service mysql stop

## Start/Restart Xampp Server

sudo /opt/lampp/lampp start

sudo /opt/lampp/lampp restart

## Store Query Data in Cache

```php
   $users = Cache::rememberForever("cache_name", function(){
      return User::all();
   });
```

## File Upload

- Store Image in DataBase

```php
   $profilePic = $request->file('image_name')->store('image_name',['disk' => 'public']);
```

- Fetch Image

```php
   {{ url(Storage::url($image_name)) }}
```

- Delete Image

```php
   $image = Storage::delete('public'.'/'.$image_name);
```