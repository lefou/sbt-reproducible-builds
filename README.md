Experimental plugin to make sbt builds more reproducible.

See also: https://reproducible-builds.org/

Overrides the `packageBin` task to post-process the result and
apply the strippers from https://github.com/Zlika/reproducible-build-maven-plugin/

Usage
=====

* Check out this repository and do `sbt publishLocal`
* Then add to your `project/plugins.sbt`: `addSbtPlugin("net.bzzt" % "sbt-reproducible-builds" % "0.2")`
* And to `build.sbt`: `enablePlugins(ReproducibleBuildsPlugin)`

