---
title: Installing the OrgManager Developer Version
---

To install the OrgManager Development Version, follow this steps:

## 1. Download beta version

Open your terminal and run

``` bash
git clone https://github.com/orgmanager/orgmanager
```

## 2. Add OrgManager to your server

!!! warning
# This step depends on your server
This step is different depending on the server you use. Normally you can get the process by searching "How to setup Laravel with X" and skipping the laravel install part. Instructions for hotel are provided, as it is the recommended server for development.
!!!

### Setup instructions for [hotel](https://github.com/typicode/hotel):

Open the OrgManager folder with the terminal/console and run

``` bash
hotel add 'php artisan serve --port $PORT'
```

Now, if you configured custom domains, you can now access `orgmanager.{yourtld}`. If you didn't, access `localhost:2000` and click OrgManager. Yeah, it should be showing that error page, don't worry :smile:

## 3. Setup .env

Copy the `.env.example` file to an `.env` file. Open the .env file with your favourite text editor/IDE and fill the database, reCaptcha and GitHub settings (you can leave the rest empty).

## 4. Finish the setup
Open the orgmanager folder with the terminal/console and run

``` bash
composer update
```
and

``` bash
php artisan app:install
```

## 5. Done!
You have now the OrgManager beta version up an running in your server! (Note that OrgManager is not auto-updated, read the updating section for more info).