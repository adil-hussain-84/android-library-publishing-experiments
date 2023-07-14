# Demonstration of an Android library which has a single publication variant

This Android library module demonstrates how to define a library which has a single publication variant.

See the [build.gradle](build.gradle) file for all the details. Pay attention to the `android.publishing` block in particular.

When you run the `publishReleasePublicationToBuildFolderRepository` Gradle task,
you'll see that the library is published in the `build/repository` folder together with its sources and javadoc supporting files.