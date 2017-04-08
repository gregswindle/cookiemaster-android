> Native Android extraction from `com.cordova.plugins.cookiemaster.CookieMaster` for reuse in native Android as well as Cordova.

[![License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://www.opensource.org/licenses/MIT)
[![Build Status](http://img.shields.io/travis/gregswindle/cookiemaster-android.svg?style=flat&branch=master)](https://travis-ci.org/gregswindle/cookiemaster-android)
[![Coverage Status](https://img.shields.io/coveralls/gregswindle/cookiemaster-android.svg?style=flat)](https://coveralls.io/r/gregswindle/cookiemaster-android?branch=master)
[![Greenkeeper badge](https://badges.greenkeeper.io/gregswindle/cookiemaster-android.svg)](https://greenkeeper.io/)

## 1. Features

### 1.1. Get a cookie by URL and name

### 1.2. Set a cookie by URL and name

### 1.3. Clear all cookies

## 2. Setup

Releases are published to [bintray jcenter](https://bintray.com/gregswindle/cookiemaster-android/cookiemaster-android/) and
[maven central](https://maven-badges.herokuapp.com/maven-central/com.verizon.api/cookiemaster-android).

<!---
[![JCenter](https://img.shields.io/bintray/v/gregswindle/cookiemaster-android/cookiemaster-android.svg?label=jcenter)](https://bintray.com/gregswindle/cookiemaster-android/cookiemaster-android/_latestVersion)
[![Maven Central](https://img.shields.io/maven-central/v/com.verizon.api/cookiemaster-android.svg?style=flat)](https://maven-badges.herokuapp.com/maven-central/com.verizon.api/cookiemaster-android)
-->

### 2.1. Maven

```xml
<dependency>
  <groupId>com.verizon.api</groupId>
  <artifactId>cookiemaster-android</artifactId>
  <version>0.1.0</version>
</dependency>
```

### 2.2. Gradle

```groovy
compile 'com.verizon.api:cookiemaster-android:0.1.0'
```

## 3. Snapshots

You can use snapshot versions through [JitPack](https://jitpack.io).

3.1. Go to [JitPack project page](https://jitpack.io/#gregswindle/cookiemaster-android).

3.2. Select `Commits` section and click `Get it` on commit you want to use (top one - the most recent).

3.3. Follow displayed instructions: add repository and change dependency (NOTE: due to JitPack convention artifact group will be different).

## 4. Recommended prerequisites

The following dependencies are recommended for consistent build, test, and deploy tasks:

### 4.1. [`Homebrew`](https://brew.sh/)

Install [`Homebrew`](https://brew.sh/):
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### 4.2. [`jenv`](http://www.jenv.be/)

Install [`jenv`](http://www.jenv.be/):

```
$ brew install jenv
```

### 4.3. `java`

Install [`Java`](http://davidcai.github.io/blog/posts/install-multiple-jdk-on-mac/) from a Terminal:

```
$ brew cask install java
```

> #### :white_check_mark: Install several versions of `Java`
>
> If you want to test this library on several versions of `Java`, the article [_Install Multiple Java Versions on Mac_](http://davidcai.github.io/blog/posts/install-multiple-jdk-on-mac/) provides clear yet detailed instructions.

### 4.4. [`gradle`](https://gradle.org/install#with-homebrew)

Install [`gradle`](https://gradle.org/install#with-homebrew) for automated build and dependency management:

```
$ brew install gradle
```

## 5. Reports :chart_with_upwards_trend:

### 5.1. Code quality and test reports

Use the following command to run code quality plugins and tests. If quality checks were activated (asked during generation) do check before pushing to avoid build failures on travis. Moreover, it's easy to always keep everything clean instead of doing it before release.

```
$ ./gradlew check
```

### 5.2. Project dependencies in a Terminal

Check whether your project dependencies are valid and prints a version analysis report to console.

```
$ ./gradlew dependencyUpdates
```

### 5.3. Project dependencies tree in a Terminal

Print the product's dependency tree in your console.

```
$ ./gradlew dependencies
```

### 5.4. Dependency reports for Web browsers

Generate a _Dependency Report_ in `HTML` and launch it in your default browser.

> ##### :white_check_mark: Analyze dependency conflicts
>
> To analyze conflicts, click on dependency name to activate a [`dependencyInsight`](http://www.gradle.org/docs/current/groovydoc/org/gradle/api/tasks/diagnostics/DependencyInsightReportTask.html) pop-up in the _Dependency Report_.

```
$ ./gradlew showDependenciesTree
```

## 6. Dependency management

:link: Install libraries to your local `maven` repository. Useful for referencing by other projects (for testing without releasing library).

```
$ ./gradlew install
```

## 7. Deployment

:globe_with_meridians: Publish the library to [jFrog Bintray](https://bintray.com/) (and therefore the world).

> #####  :warning: Read the [_Release process_](https://github.com/xvik/generator-lib-java#release-process) first!
>
> Before publishing the library, [read the section _Release process_](https://github.com/xvik/generator-lib-java#release-process) in the `generator-lib-java` README.md.

```
$ ./gradlew release
```

---
[![java lib generator](http://img.shields.io/badge/Powered%20by-%20Java%20lib%20generator-green.svg?style=flat-square)](https://github.com/xvik/generator-lib-java)
