# mod-lang-clojure

A fledgling Vert.x language implementation for Clojure

## Usage

First, you'll need to [install Vert.x](http://vertx.io/install.html).

The latest stable release is *0.4.0*. Until this module becomes part
of Vert.x proper, you will need to make Vert.x aware of it by editing
`VERTX_HOME/conf/langs.properties` and adding:

    clojure=io.vertx~lang-clojure~0.4.0:io.vertx.lang.clojure.ClojureVerticleFactory
    .clj=clojure


Every commit triggers a [CI](https://vertx.ci.cloudbees.com/job/vert.x-mod-lang-clojure/)
build, and we publish a SNAPSHOT when that succeeds. So if you would
rather run the latest commit, update your `langs.properties` with:

    clojure=io.vertx~lang-clojure~0.5.0-SNAPSHOT:io.vertx.lang.clojure.ClojureVerticleFactory
    .clj=clojure

**Note that this module only works with Vert.x 2.1M2 or greater.**

## Documentation

For 0.4.0:

* [User Manual](https://github.com/vert-x/mod-lang-clojure/blob/0.4.0/docs/core_manual_clojure.md)
* [API docs](http://vertx.io/mod-lang-clojure/docs/0.4.0/index.html)

For HEAD:

* [User Manual](docs/core_manual_clojure.md)
* [API docs](https://vertx.ci.cloudbees.com/job/vert.x-mod-lang-clojure/lastSuccessfulBuild/artifact/api/target/html-docs/index.html)

## Examples

See [examples/README.md](examples/README.md).

## License

mod-lang-clojure is licensed under the Apache License, v2.0. See
[LICENSE.txt](LICENSE.txt) for details.
