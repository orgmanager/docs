---
title: Installing the OrgManager Stable Version
---

To install the OrgManager Stable Version, follow this steps:

## 1. Download latest stable version

Download [the lastest release](https://github.com/orgmanager/orgmanager/releases/latest) and unzip it on your server.

## 2. Add OrgManager to your server

!!! warning
# This step depends on your server
This step is different depending on the server you use. Normally you can get the process by searching "How to setup Laravel with X" and skipping the laravel install part.
!!!

If you try to access OrgManager at his step, it should show an error. Don't worry :smile: 

## 3. Setup .env

Copy the `.env.example` file to an `.env` file. Open the .env file with your favourite text editor/IDE and fill the database, reCaptcha and GitHub settings. (You can leave the rest as they are, although it is recommended setting up [Sentry](https://sentry.io/) in production).

!!! warning
# Remember to disable debug mode!
Remember to set `DEBUG` to `false` and `APP_ENV` to `prod`.
!!!

## 4. Finish the setup

Open the OrgManager folder with the terminal/console and run

``` bash
composer update
```
and

``` bash
php artisan app:install
```

## 5. Done!
You have now the latest OrgManager stable version up and running in your server! (Note that OrgManager is not auto-updated, read the updating section for more info).