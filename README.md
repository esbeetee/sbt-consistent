# sbt-consistent

SBT plug-in to enable Maven-compliant SBT plug-ins, especially for the corporate world.

# How this plug-in will be used

To an SBT project, add `project/project/plugins.sbt` (as it's a plug-in that loads before other plug-ins)

```
libraryDependencies += "io.github" %% "sbt-consistent" % "0.0.2"
```

Once this plug-in is added, automatically the consumer will be unable to load inconsistent plug-ins.
In order to verify this, we have an SBT plug-in test to verify, as per below;

https://www.scala-sbt.org/1.x/docs/Testing-sbt-plugins.html

https://github.com/daniel-shuy/scripted-scalatest-sbt-plugin