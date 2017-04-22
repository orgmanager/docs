excerpt: Here you can find the steps you need to follow to install the OrgManager Development Version
slug: prod-installing

To install the OrgManager Stable Version, just follow this steps:
[block:api-header]
{
  "type": "basic",
  "title": "1. Download latest stable version"
}
[/block]

Download [the lastest release](https://github.com/orgmanager/orgmanager/releases/latest) and unzip it on your server.
[block:api-header]
{
  "type": "basic",
  "title": "2. Add OrgManager to your server"
}
[/block]

[block:callout]
{
  "type": "warning",
  "title": "This steps depend on your server",
  "body": "This step is different depending on the server you use. Normally you can get the process by searching \"How to setup Laravel with X\" and skipping the laravel install part."
}
[/block]
If you try to access OrgManager at his step, it should show an error. Don't worry :smile: 
[block:api-header]
{
  "type": "basic",
  "title": "3. Setup .env"
}
[/block]
Copy the `.env.example` file to a `.env` file. Open the .env file with your favorite text editor/IDE and fill the database, reCaptcha and GitHub settings. (You can leave the rest as they are, although it is recommended setting up [Bugsnag](https://www.bugsnag.com/) in production).
[block:callout]
{
  "type": "warning",
  "title": "Remember to disable debug mode!",
  "body": "remember to set `DEBUG` to `false` and `APP_ENV` to `prod`."
}
[/block]

[block:api-header]
{
  "type": "basic",
  "title": "4. Finish the setup"
}
[/block]
Open the OrgManager folder with the terminal/console and run

```sh
composer update
```
and

```sh
php artisan app:install
```
[block:api-header]
{
  "type": "basic",
  "title": "5. Done!"
}
[/block]
You have now the latest OrgManager stable version up an running in your server! (Note that OrgManager is not auto-updated, read the updating section for more info).