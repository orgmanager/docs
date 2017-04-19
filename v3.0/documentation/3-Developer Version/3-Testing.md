excerpt: Learn how to setup and run the OrgManager Feature & Unit Tests
slug: testing

We use the Laravel testing functionalities and PHPUnit to add automated testing to OrgManager.
[block:api-header]
{
  "title": "Setting up the testing enviroment"
}
[/block]
By default, the tests will run in a special database called `orgmanager_test` in `localhost` with username `root` and password `root`. If you need to change this, edit the `.env.testing` file. This is an example of a customized `.env.testing` file:

``` php
APP_ENV=testing
APP_KEY=base64:GIkaQ57IIVtTeTQOIh7eAFo1FAcoWkfwYPkfcOyusW4=

DB_CONNECTION=travis

DB_TEST_HOST=database_host
DB_TEST_DATABASE=database_name
DB_TEST_USERNAME=database_username
DB_TEST_PASSWORD=database_password

CACHE_DRIVER=array
SESSION_DRIVER=array
QUEUE_DRIVER=sync
```

Once you've customized your .env.testing file, you have to migrate the database to your test database. You can do this by running 
``` sh
php artisan migrate --env=testing
```
[block:api-header]
{
  "title": "Running the tests"
}
[/block]

To run the tests, just run
``` sh
composer test
```