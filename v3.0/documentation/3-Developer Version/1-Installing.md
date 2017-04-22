excerpt: Here you can find the steps you need to follow to install the OrgManager Development Version
slug: dev-installing

To install the OrgManager Development Version, just follow this steps:
[block:api-header]
{
  "type": "basic",
  "title": "1. Download beta version"
}
[/block]

Open your terminal and run
```
git clone https://github.com/orgmanager/orgmanager
```
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
  "body": "This step is different depending on the server you use. Normally you can get the process by searching \"How to setup Laravel with X\" and skipping the laravel install part. Instructions for hotel are provided, as it is the recommended server."
}
[/block]
### Setup instructions for [hotel](https://github.com/typicode/hotel):

Open the OrgManager folder with the terminal/console and run

```sh
hotel add 'php artisan serve --port $PORT'
```

Now, if you configured custom domains, you can now access `orgmanager.{yourtld}`. If you didn't, access `localhost:2000` and click OrgManager. Yeah, it should be showing that error page, don't worry :smile:
[block:api-header]
{
  "type": "basic",
  "title": "3. Setup .env"
}
[/block]
Copy the `.env.example` file to a `.env` file. Open the .env file with your favorite text editor/IDE and fill the database, reCaptcha and GitHub settings (you can leave the rest as they are).
[block:api-header]
{
  "type": "basic",
  "title": "4. Finish the setup"
}
[/block]
Open the orgmanager folder with the terminal/console and run

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
You have now the OrgManager beta version up an running in your server! (Note that OrgManager is not auto-updated, read the updating section for more info).