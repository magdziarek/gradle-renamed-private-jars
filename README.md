# gradle-renamed-private-jars

An example project showing how to use Snyk to scan unmanaged dependencies (Java archive files) using Gradle. The dependencies are jar files that have the same content and sha1 value as the ones on Maven Central but their group id and artifact id have been modified. They are privately hosted.

## Usage

## Notes

To make this work you need a gradle.properties file that contains the values:

```s
nexusUrl=<https://your.private/repo>
nexusUsername=<your-username>
nexusPassword=<your-password>
```

To support older version of Gradle `apply plugin: <name>` is used instead of `plugins`.

This repository works with the following major version of Gradle:

- 7
- 6
- 5

but is configured to use `7.5.1` in the Gradle wrapper.
