# template

clj -X:new :template figwheel-main :name tutorial/template :args '["+deps" "--reagent"]'

with .dir-locals.el to connect to emacs repl. I had to restart emacs after adding this file to work properly.
## Overview

simpliest template with working emacs repl


## Development

To get an interactive development environment run:

    clojure -A:fig:build

This will auto compile and send all changes to the browser without the
need to reload. After the compilation process is complete, you will
get a Browser Connected REPL. An easy way to try it is:

    (js/alert "Am I connected?")

and you should see an alert in the browser window.

To clean all compiled files:

    rm -rf target/public

To create a production build run:

	rm -rf target/public
	clojure -A:fig:min


## License

Copyright © 2018 FIXME

Distributed under the Eclipse Public License either version 1.0 or (at your option) any later version.
