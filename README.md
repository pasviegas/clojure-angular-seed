# clojure-angular-seed

A seed project for getting started fast with Clojure and AngularJS.


## What?

A quick and easy way to get off the ground with a Clojure and AngularJS.
This project provides a minimal Clojure web server which serves up a
single-page AngularJS application and provides the beginnings of a RESTful
backend API. It also uses bower to manage front-end dependencies and grunt
to orchestrate coffee-script and sass compilation, copying files around,
starting the dev server and watching for changes to source files.


## Why?

Because it takes a while to get up and running with a
Clojure/Angular/CoffeeScript/Sass app in the first place, and that's before
you've even started to build the actual functionality of your cool new app.
This repo provides a minimal setup useful for getting straight to work
rather than spending two hours just getting to square one.


## How?
This project was set up by first generating a bare-bones
[luminus](luminusweb.net) app, then generating [yeoman](yeoman.io) angular
app and selectivly moving the good parts of the angular app over to the
clojure project. The gruntfile was built from scratch to provide only the
functionality that was needed to get the basic app working, consider it a
base from which to start work rather than a finished 'framework'.


## Prerequisites

You will need [Leiningen][1] 2.0 or above installed.

[1]: https://github.com/technomancy/leiningen

You will also need to have [nodejs](http://nodejs.org) and
[ruby](http://ruby-lang.org) installed.


## Running

To set up the project, install grunt, coffeescript and bower:
```
$ npm install -g grunt-cli bower coffee-script
```
depending on how you installed nodejs, you may need root permissions for
the above command. Subsequent commands should not be run with root
permissions.


Install the Sass ruby gem:
```
$ gem install sass
```


Then install npm and bower packages:
```
$ npm install

$ bower install
```


Finally, to run the development server:
```
$ grunt server
```


To make the process of starting your new project easier, you can instantly
change the name of the project by running:
```
$ ./bin/change-project-name.sh <name>
```


For example: `$ ./bin/change-project-name.sh wibble` will change your
project and its clojure modules to be called 'wibble' rather than the
default 'cljang'.


## Future

In future, expect to see:
* tests, both for the angular frontend and for the clojure api
* easy deployment/packaging
* other tiny improvements
* relentless yak shaving


## License

Copyright © 2013 Shane Kilkelly, [MIT License](opensource.org/licenses/MIT)
