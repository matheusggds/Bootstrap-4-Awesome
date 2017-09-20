# Bootstrap 4 Awesome
> I almost everytime use BS4 + FontsAwesome + Sass + Gulp on my projects, cause for me they ~~born~~ are perfect for each other. So i am sharing it for who wants to, enjoy!

## Init
> https://github.com/matheusggds/Bootstrap-4-Awesome.git

## Editing
Add your own CSS styles to `/sass/custom/custom.scss`

To overwrite Bootstrap base variables just add your own value to: `/sass/custom/custom_variables.scss`

For example:

```
$brand-primary: #fefefe
```

 the **$brand-primary** variable is used by Bootstrap. Add your own color in `/sass/custom/custom_variables.scss` to overwrite it.

That will change automatically all elements who use this variable. It will be outputted into: `assets/css/style.min.css` and `assets/css/style.css`

So you have one clean CSS file at the end and just one request.

### Installing Dependencies
- Make sure you have installed [Node.js](https://nodejs.org/), [Gulp](https://gulpjs.com/), and Browser-Sync [1] on your computer globally
- Then open your terminal and browse to the location of your project
- Run: `$ npm install` then: `$ gulp copy-assets`

### Running
To work and compile your Sass files on the fly start:

- `$ gulp watch`

Or, to run with Browser-Sync:

- First change the browser-sync options to reflect your environment in the file `/gulpfile.js` in the beginning of the file:
```javascript
var browserSyncOptions = {
    proxy: "localhost/project_name/", // <----- CHANGE HERE
    notify: false
};
```
- then run: `$ gulp watch-bs`

[1] Visit [http://browsersync.io](http://browsersync.io) for more information on Browser Sync
