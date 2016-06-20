harp-browserify-babel
=====================

A harp boilerplate with browserify and es6 (through babelify) support.
Javascript bundles are split into small per page bundles and one big 'common.js' file using factor-bundle.
Production code is minified through uglifyjs.

Use it:
=======

Either install harp globally ...

```
npm i -g harp
```
... and use this repo as a boilerplate:

```
harp init -b janruehling/harp-browserify-babel
```

... or clone the repository.

Then do ...

```
npm install
npm run dev
```

... to start a watcher that monitors the **/src** directory.
ONLY edit or add files to the **/src** directory, any changes will be copied to the **/public** folder and harp does its magic from there.
Once you are happy with your site do ...

```
npm run prod
```

... and browserify will minify the Javascript files before harp compiles all files and puts them into **/www**
