# Demonstration of an Android library which has multiple publication variants

This Android library module demonstrates how to define a library which has multiple publication variants.

See the [build.gradle](build.gradle) file for all the details. Pay attention to the `android.publishing` block in particular.

Unlike [library1](../library1) which offers `publishRelease...` Gradle tasks only,
you'll notice that this library offers both `publishDebug...` and `publishRelease...` Gradle tasks.

One problem to be aware of when defining a library as in this module (i.e. with multiple publication variants)
is that the `publishDebug...` and `publishRelease...` Gradle tasks publish the library without its supporting javadoc files.
I have raised this as a bug in Google's IssueTracker [here](https://issuetracker.google.com/issues/291106650).
