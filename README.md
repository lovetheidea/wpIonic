# wpIonic

A mobile app that uses the Ionic Framework, and integrates with WordPress through the WP-API.

Features:

- Gets posts through WP-API
- Pull to refresh
- Infinite scroll
- App intro
- WordPress login (needs custom code on your site to do anything)
- More coming soon

## Demo

https://github.com/scottopolis/wpIonic/blob/master/demo-video.gif

## How to use this template

### 1. Install Ionic

```bash
$ npm install -g ionic cordova
$ npm install ios-sim -g
```

### 2. Install WordPress REST API (Version 2)

Please install [WordPress REST API (Version 2)](https://ja.wordpress.org/plugins/rest-api/) into your WordPress site.

### 3. Start a project

```bash
$ ionic start myApp https://github.com/lovetheidea/wpIonic/
$ cd myApp
$ ionic platform add ios
$ ionic platform add android
```

Go to www/js/controllers.js and change $rootScope.url to your website:

```javascript
.constant( 'config', {
  api: 'http://example.com/wp-json/wp/v2' // API URL of your WordPress
} )
```

If you want to try quickly, you can skip here.

### 4. Run it

Run your app on iOS simulator.

```bash
$ ionic emulate ios
```

Or run on your browser.

```bash
$ ionic serve
```


## How to setup

Blog post here: http://scottbolinger.com/ionic-wordpress-app/

1. Install and activate the WP-API v2 plugin on your WordPress website [https://wordpress.org/plugins/rest-api/]
2. Go to www/js/controllers.js and change $rootScope.url to your website
3. Load index.html in Safari, or compile app with Phonegap

**Props to [https://github.com/modemlooper]**
