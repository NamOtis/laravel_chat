# Laravel realtime chatting application

Very simple php based chatting application

# Installation
1. Clone this repo
```
https://github.com/samironbarai/laravel_chat
```

2. Install composer packages
```
cd laravel-chat
composer install
```

* make a copy of .env.example and rename to .env
* php artisan key:generate
* put database credentials in .env file
* run php artisan migrate
* to insert users and messages data run php artisan tinker
* factory(App\User::class, 30)->create();
* factory(App\Message::class, 500)->create();
* login to https://pusher.com/ and create new app
* put pusher credentials to .env file
* replace PUSHER_APP_KEY in your app.blade.php
```ruby
var pusher = new Pusher('49f3ba8c9d3adab2613e', {
    cluster: 'ap2',
    forceTLS: true
});
```
