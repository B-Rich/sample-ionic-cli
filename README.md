# Ionic CLI

### Features
More info here: http://ionic.io/discover, http://ionicframework.com/ and here: http://ionicframework.com/docs/cli/
- Ionic Lab `ionic serve --lab`
- LiveReload on Device `ionic run --livereload`
- Resource (icons/splash) Generation `ionic resources`
- Browsers/Crosswalk http://ionicframework.com/docs/cli/browsers.html
- Ionic Platform (beta) http://ionic.io/
  - User Auth / Data - http://docs.ionic.io/docs/user-overview
  - Push - http://docs.ionic.io/docs/push-overview
  - Deploy / Upload / Ionic View App `ionic upload` http://docs.ionic.io/docs/deploy-overview
  - Analytics - http://docs.ionic.io/docs/analytics-auto-tracking
  - Package (Build/Release Service) - http://docs.ionic.io/docs/package-overview

### Downsides/questions
- why not a generator?
  - would be great to provide hooks for developers to automate setup of their ionic projects according to their own needs
- no `--no-open` :(
- integration
  - no out-of-the-box git integration
    - `www/lib`, `.io-config.json`, `www/css` (when using sass) not in gitignore
  - cumbersome sass integration - http://ionicframework.com/docs/cli/sass.html
  - no good integration with gulp/bower/yeoman
    - bower components not automatically added to index
    - new files / scss not automatically added to index
  - no \*lint integration
  - no testing integration
- obscured cordova version/integration
  - source files in `www/`
  - build process?
  - https://github.com/driftyco/ionic-cli/blob/master/lib/ionic/cordova.js#L10
  - https://github.com/driftyco/ionic-app-lib/blob/master/package.json#L50
- no sub-generators
- file structure not compatible with
  - cordova?
  - components or google app recommendation?


----

Ionic App Base
=====================

A starting project for Ionic that optionally supports using custom SCSS.

## Using this project

We recommend using the [Ionic CLI](https://github.com/driftyco/ionic-cli) to create new Ionic projects that are based on this project but use a ready-made starter template.

For example, to start a new Ionic project with the default tabs interface, make sure the `ionic` utility is installed:

```bash
$ npm install -g ionic
```

Then run:

```bash
$ ionic start myProject tabs
```

More info on this can be found on the Ionic [Getting Started](http://ionicframework.com/getting-started) page and the [Ionic CLI](https://github.com/driftyco/ionic-cli) repo.

## Issues
Issues have been disabled on this repo, if you do find an issue or have a question consider posting it on the [Ionic Forum](http://forum.ionicframework.com/).  Or else if there is truly an error, follow our guidelines for [submitting an issue](http://ionicframework.com/submit-issue/) to the main Ionic repository.
