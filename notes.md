Things to look at

Graph of sources
CrossCLJ — what's used and not used in ecosystem?
clj use vs cljs?
its dependencies (basically all up to date)
try out the tests — is there even a guide for how to test?


;; general comments

splitting out the examples and the website builder would make this simpler to understand
what would clojure.spec do for it?
interop could be split out
TIL reagent interop macros might come in handy
uses Makefile for common tasks rather than leiningen
imports stuff into core to make it easily accessible


;; testing
could definitely benefit from runner not in browser
here's how I get them running:


~/C/c/reagent (master) [130]> lein with-profile fig,test figwheel
Figwheel: Validating the configuration found in project.clj

Figwheel: Configuration Valid. Starting Figwheel ...
Figwheel: Starting server at http://0.0.0.0:3449
Figwheel: Watching build - client
Compiling "outsite/public/js/main.js" from ("src" "demo" "examples/todomvc/src" "examples/simple/src" "examples/geometry/src" "test")...
Successfully compiled "outsite/public/js/main.js" in 8.432 seconds.
Figwheel: Starting CSS Watcher for paths  ["site/public/css"]


Testing reagenttest.testratom
core.cljs:150
Testing reagenttest.testtrack
core.cljs:150
Testing reagenttest.testwithlet
core.cljs:150
Testing reagenttest.testratomasync
core.cljs:150
Testing reagenttest.testinterop
core.cljs:150
Testing reagenttest.testreagent
core.cljs:150
Testing reagenttest.testwrap
core.cljs:150
Testing reagenttest.testcursor
core.cljs:150
Ran 101 tests containing 2267 assertions.
core.cljs:150 0 failures, 0 errors.