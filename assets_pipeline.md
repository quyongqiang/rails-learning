# assets pipeline

### Assets in Rails
- images
- JavaScript Files
- CSS Files

`http://localhost:3000/assets/application.css`

### purpose of assets
- Minify
- Compile
scss -> css
- Fingerprint
md5 string in file name, for invalidate browser cache

### what is assets pipeline?
```
combine all the css files into a single file, also js files are combined.

```
### monolith file



### Where to put our assets
```
app/assets
lib/assets
vender/assets
```

### manifest files
```
decide which file to be get combined and send to

to the browser.
application.js
application.css

//= require posts
//= require tree .

```

### show assets path
```
Rails.application.config.assets.paths
```

### precompile assets
```
rake assets:precompile
```

### What is turbolinks ?


### What is sprockets?
https://github.com/rails/sprockets

```
Sprockets is a Ruby library for compiling and serving web assets. It features declarative dependency management for JavaScript and CSS assets, as well as a powerful preprocessor pipeline that allows you to write assets in languages like CoffeeScript, Sass and SCSS.
```

### development and production difference
development
- compile on every request
- minify is off
- fingerprint is off

production
- compile once at deploy
- minify is on
- fingerprint is on
