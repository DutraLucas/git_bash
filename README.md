# git_bash


---

### Manual installation
* Clone or Download the Zip file from Github
* Copy the `Gallery` folder to your app plugins folder: `app/Plugin/`
* Rename the `app/Plugin/Gallery/Config/config.php.install` file to **config.php**
* Import the SQL file `app/Plugin/Gallery/Config/cakegallery.sql` to your database
* Open your `app/Config/bootstrap.php` file and add the following code

```php
CakePlugin::load(array(
	'Gallery' => array(
   	'bootstrap' => true,
    'routes' => true
)));
```
* Create a **gallery** folder inside `app/webroot/files` and give it writable permissions. (`app/webroot/files/gallery`)

* Check at `http://your-app-url/gallery` to see your plugin working.

---