PostCSS Plugins
===============

list of content
---------------
- [CSS](#css)
- [SVG](#svg)
- [Assets](#assets)

----

CSS
----
#### [cssnano](https://github.com/ben-eb/cssnano#--------------------)
PreCSS is a tool that allows you to use Sass-like markup in your CSS files.
```bash
	$ npm i -D cssnano
```

#### [PreCSS ](https://github.com/jonathantneal/precss#precss-)
PreCSS is a tool that allows you to use Sass-like markup in your CSS files.
```bash
	$ npm i -D postcss
```
```javascript
var postcss = require('gulp-postcss');

gulp.task('css', function () {
    return gulp.src('./css/src/*.css').pipe(
        postcss([
            require('precss')({ /* options */ })
        ])
    ).pipe(
        gulp.dest('./css')
    );
});
```
####[Autoprefixer ](https://github.com/postcss/autoprefixer#autoprefixer-)
**PostCSS plugin to unwrap nested rules like how Sass does it.**
```bash
	$ npm i -D autoprefixer
```

####[postcss-nested](https://github.com/postcss/postcss-nested#postcss-nested-)
**PostCSS plugin to unwrap nested rules like how Sass does it.**
```bash
	$ npm i -D postcss-nested
```

####[postcss-simple-vars](https://github.com/postcss/postcss-simple-vars#postcss-simple-variables-)
**PostCSS plugin for Sass-like variables.**
```bash
	$ npm i -D postcss-simple-vars
```

#### [Stylelint](https://github.com/stylelint/stylelint#stylelint)
A mighty, modern CSS linter that helps you enforce consistent conventions and avoid errors in your stylesheets.
```bash
	$ npm i -D stylelint
```

#### [Oldie](https://github.com/jonathantneal/oldie#oldie-)
Oldie tranforms CSS to be compatible with old Internet Explorer.
```bash
	$ npm i -D oldie
```
#### [PostCSS Browser Reporter](https://github.com/postcss/postcss-browser-reporter#postcss-browser-reporter-)
PostCSS plugin to report warning messages right in your browser.
```bash
	$ npm i -D postCSS-browser-reporter
```
![Postcss-browser-reporter – warnings from other postcss plugins in your browser](http://postcss.github.io/postcss-browser-reporter/screenshot.png)
----------

SVG
----
#### [postcss-inline-svg ](https://github.com/TrySound/postcss-inline-svg#postcss-inline-svg-)
plugin to reference an SVG file and control its attributes with CSS syntax.
```bash
	$ npm i -D postcss-base64
```

#### [postcss-base64](https://github.com/jelmerdemaat/postcss-base64#use)
postcss-base64, a PostCSS plugin, replaces urls or values inside url() functions with their base64 encoded strings.
```bash
	$ npm i -D postcss-inline-svg
```

```javascript
	var gulp = require('gulp'),
	    postcss = require('gulp-postcss'),
	    base64 = require('postcss-base64');

	gulp.task('css', function () {
	  gulp.src('test.css')
	      .pipe(postcss([
	        base64({
	          extensions: ['.svg']
	        })
	      ]))
	      .pipe(gulp.dest('output/'));
	});
```

Assets
------
#### [PostCSS Assets](https://github.com/assetsjs/postcss-assets#table-of-contents)
PostCSS Assets is an asset manager for CSS. It isolates stylesheets from environmental changes, gets image sizes and inlines files.
```bash
	$ npm i -D postcss-assets
```

#### [postcss-copy](https://github.com/geut/postcss-copy#postcss-copy)
An async postcss plugin to copy all assets referenced in CSS files to a custom destination folder and updating the URLs.
```bash
	$ npm i -D postcss-copy
```

#### [PostCSS Easysprite](https://github.com/glebmachine/postcss-easysprites#postcss-easysprite--)
Just append #spritename to the end of image url. No complicated mechanism or strict folder structure.
```bash
	$ npm i postcss-easysprites
```

```css
.arrow {
  background-image: url('/images/arrow-next.png#elements');
}
.arrow:hover {
  background-image: url('/images/arrow-next_hover.png#elements');
}

@media only screen and (-webkit-min-device-pixel-ratio: 1.5) {
  .arrow {
    background-image: url('images/arrow-next@2x.png#elements');
  }
  .arrow:hover {
    background-image: url('/images/arrow-next_hover@2x.png#elements');
  }
}

@media only screen and (-webkit-min-device-pixel-ratio: 2.5) {
  .arrow {
    background-image: url('images/arrow-next@3x.png#elements');
  }
  .arrow:hover {
    background-image: url('images/arrow-next_hover@3x.png#elements');
  }
}
```
#### [PostCSS postcss-mq-keyframes](https://github.com/TCotton/postcss-mq-keyframes#postcss-postcss-mq-keyframes)
This plugin will move any keyframe animations from inside media queries to the bottom of the CSS file.
```bash
	$ npm i -D postcss-mq-keyframes
```

#### [postcss-instagram](https://github.com/azat-io/postcss-instagram#postcss-instagram)
```bash
	$ npm install postcss-instagram --save
```
