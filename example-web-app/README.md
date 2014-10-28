# example.webapp

A single page web app using [leaven][leaven] components from
[bakery][bakery].

## Usage

```
$ cd ~/tmp
$ git clone https://github.com/palletops/bakery.git
$ git checkout master
$ cd example-web-app
$ lein cljsbuild once
$ lein repl
user=> (start {})    ;; starts webserver on port 3000
user=> (start-cljs-repl!)    ;; now refresh your browser
;; clojurescript repl started
```

Clone the project, and checkout the `master` branch (to run the
default `develop` branch you would need to `lein install` the top
level [bakery][bakery] project first).

Run `lein cljsbuild once`.

Start a repl and run `(start {})` to start the webserver on port 3000.

Call `(start-cljs-repl!)` and refresh your browser to create a
clojurescript repl.

Uses httpkit, sente, weasel, storage-atom, secretary, om-bootstrap
among other libraries.

## License

Copyright © 2014 Hugo Duncan

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.

[bakery]:https://github.com/palletops/bakery "bakery components for leaven"
[leaven]:https://github.com/palletops/leaven "leaven component library"
