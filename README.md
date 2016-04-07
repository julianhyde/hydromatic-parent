# hydromatic-parent
Parent POM for net.hydromatic projects

# How to release

To make a release of a project that uses hydromatic-parent as its
parent POM, use the following steps.

```bash
$ git clean -nx
$ mvn clean
$ mvn -Prelease release:prepare
$ mvn -Prelease release:perform
```

Open http://oss.sonatype.org, log in, find the repository you just
published, close, then release. The artifacts should appear in Maven
Central in about an hour.