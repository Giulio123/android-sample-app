android-sample-app
==================

[work in progress]

This sample android app demonstrates how to setup [Robolectric](http://robolectric.org/) to write/run tests and how to create a continuous integration/deployment setup either in Wercker/CircleCI

#### Integrating Robolectric

Add `junit` and `robolectric` as dependencies in [app/build.gradle](https://github.com/multunus/android-sample-app/blob/master/app/build.gradle)

``` gradle
dependencies {
    ...
    androidTestCompile 'junit:junit:4.12'
    androidTestCompile "org.robolectric:robolectric:3.0"
}
```
