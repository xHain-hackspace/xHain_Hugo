# xHain_Hugo

[![wercker status](https://app.wercker.com/status/4374b5664faf5920c218c1b06618581a/m/master "wercker status")](https://app.wercker.com/project/byKey/4374b5664faf5920c218c1b06618581a)

# Getting started

cf. http://xhain.s3-website.eu-central-1.amazonaws.com/

For MacOS:
* Install brew (for installing the rest)
* Install go: ``brew install go``
* Install hugo: ``brew install hugo``
* Run hugo to generate HTML: ``brew install hugo``

For Windows/Linux:
* Install hugo: [http://gohugo.io/](Hugo Website)

# Editing Site

Just edit the content in the "content"-folder


# Development

In order to develop or make changes to the theme you will need to have the sass compiler and bourbon both installed.

To check installation run the following commands from a terminal and you should see the `> cli output` but your version numbers may vary.

** SASS **
```bash

sass -v
> Sass 3.3.4 (Maptastic Maple)
```
If for some reason SASS isn't installed then either follow the instructions from the [Sass install page](http://sass-lang.com/install) or run `bundle install` in the project root.

** Bourbon **
```bash

bourbon help
> Bourbon 3.1.8
```
If Bourbon isn't installed follow the installation instructions on the [Bourbon website](http://bourbon.io) or run `bundle install` in the project root.

Once installation is verified we will need to go mount the bourbon mixins into the `scss` folder.

From the project root run `bourbon install` with the correct path
```bash
bourbon install --path static/scss
> bourbon files installed to static/scss/bourbon/
```

Now that we have the bourbon mixins inside of the `scss` src folder we can now use the sass cli command to watch the scss files for changes and recompile them.

```bash
sass --watch static/scss:static/css
>>>> Sass is watching for changes. Press Ctrl-C to stop.
```

To minify the css files use the following command in the static folder

```bash
curl -X POST -s --data-urlencode 'input@static/css/uno.css' http://cssminifier.com/raw > static/css/uno.min.css
```

