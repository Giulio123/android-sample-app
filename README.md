android-sample-app
==================

[work in progress]

This sample android app demonstrates how to setup [Robolectric](http://robolectric.org/) to write/run tests and how to create a continuous integration/deployment setup either in Wercker/CircleCI

#### Creating an Android Project in Android Studio

Create a blank activity project in Android Studio with MainActivity. Android Studio uses a gradle-based build setup which also makes it easy to run Robolectric tests .

#### Integrating Robolectric

Add `junit` and `robolectric` as dependencies in [app/build.gradle](https://github.com/multunus/android-sample-app/blob/master/app/build.gradle)

``` gradle
dependencies {
    ...
    compile 'junit:junit:4.12'
    compile "org.robolectric:robolectric:3.0"
}
```

#### Writing Your First Test

Test files reside in `app/src/test/` directory. For now, create a test file for MainActivity, [MainActivityTest](https://github.com/multunus/android-sample-app/blob/master/app/src/test/java/com/multunus/cdapp/MainActivityTest.java)

#### Running Robolectric Tests

You can run the tests via the terminal. Go to the root directory of the project and run:

``` bash
./gradlew clean test
```
