## Change log
----------------------

Version 2.2 (unreleased)
-------------

CHANGED:

- the source of 2.1 is on GitHub (#7): the three commits it was built from had never been pushed, and
  five of its build files (gradle/apply-gradle-files.gradle, gradle-files.list, libs.versions.toml,
  tagging.gradle, version-catalog-update.gradle) had never been committed, because .gitignore hid
  /gradle. They are merged into develop as they were built
- a pre-commit hook refuses a commit whose files Spotless would format (#1)
- CI submits the Gradle dependency graph to GitHub (#3)
- .gitignore no longer hides /gradle (#5)

Version 2.1
-------------

Released to Maven Central on 2026-08-24, built with Gradle 9.7.0 for JDK 17 (roboter-2.1.module).

CHANGED:

- built from a Gradle version catalog with bundles, and published through the Central Portal
- Gradle 9.7.0
- randomizer 10.1 at runtime (roboter-2.1.pom). randomizer before 10.5 seeds its default generator
  with the current time (GHSA-395w-fmf5-xfj3); raising it is planned for the next release

Version 2
-------------

CHANGED:

- update of jdk to version 17
- update of gradle to new version 8.4-rc-1
- update of lombok version to 1.18.30
- update of gradle plugin dependency io.freefair.gradle:lombok-plugin to new version 8.3
- update of com.github.ben-manes.versions.gradle.plugin to new version 0.48.0
- update of gradle-plugin dependency of 'com.diffplug.spotless:spotless-plugin-gradle' in version 6.21.0
- update of dependency randomizer to new minor version 10.1

Version 1
-------------

ADDED:

- new CHANGELOG.md file created

Notable links:
[keep a changelog](http://keepachangelog.com/en/1.0.0/) Don’t let your friends dump git logs into changelogs
