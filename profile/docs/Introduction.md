# Introduction and Overview

## `scoverage` features and repositories

- [scalac-scoverage-plugin][] - the compiler plugin for Scala 2 and
  lots of other utilities (e.g. the report writers) that are used by
  the tools
- [sbt-scoverage][] - the [sbt][] plugin
- [gradle-scoverage][] - the [gradle][] plugin
- [scoverage-maven-plugin][] - the [maven][] plugin
- [sbt-coveralls][] - the sbt plugin to upload scoverage reports to
  [coveralls][]
- [sbt-scoverage-examples][] - example reports, which show how to use
  scoverage

## A little bit of history

This was build for Scala 2. Initially it was mainly a compiler plugin
that is annotating/instrumenting the Abstract Syntax Tree ([AST][]).

When you execute the code by running the tests that instrumentation
will then create the `scoverage.coverage` file. That file shows what
branches of the code have been visited and covered.

`scoverage` then features a set of report writers to turn that file
into various reports (html, xml, ...) for viewing or further
processing.

`scoverage` also features integrations with all the leading build
tools (sbt, gradle, maven, ...). There is also a [jenkins][] plugin
that is maintained by jenkins and there is support for scoverage in
[mill][].

`scoverage` provides coverage for scala, scala-js and scala-native.

To support Scala 3 the compiler plugin was merged into dotty (starting
with [3.2][merged-into-dotty]).

## Resources

- Scoverage and [SonarQube][]
- Scoverage [Tutorial][] (old)
- Scoverage [Talk][] (new)
- Developer Chat on [Gitter][]

[AST]: https://en.wikipedia.org/wiki/Abstract_syntax_tree
[coveralls]: https://coveralls.io/
[Gitter]: https://gitter.im/scoverage/scoverage
[gradle]: https://gradle.org/ 
[gradle-scoverage]: https://github.com/scoverage/gradle-scoverage
[jenkins]: https://github.com/jenkinsci/scoverage-plugin
[maven]: https://maven.apache.org/
[merged-into-dotty]: https://dotty.epfl.ch/docs/internals/coverage.html
[mill]: https://com-lihaoyi.github.io/mill/mill/0.9.9/Contrib_Modules.html#_scoverage
[sbt-coveralls]: https://github.com/scoverage/sbt-coveralls
[sbt-scoverage]: https://github.com/scoverage/sbt-scoverage
[sbt-scoverage-examples]: https://github.com/scoverage/sbt-scoverage-examples
[sbt]: https://www.scala-sbt.org/
[scalac-scoverage-plugin]: https://github.com/scoverage/scalac-scoverage-plugin
[scoverage-maven-plugin]: https://github.com/scoverage/scoverage-maven-plugin
[SonarQube]: https://blog.knoldus.com/scoverage-analysis-scala-sbt/
[Talk]: https://www.youtube.com/watch?v=SIkNgemGmYQ&ab_channel=ScalaCon
[Tutorial]: https://www.youtube.com/watch?v=oz_HcHvbp7Y&ab_channel=MelvinL
