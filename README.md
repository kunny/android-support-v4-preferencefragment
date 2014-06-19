[![Build Status](https://travis-ci.org/kunny/android-support-v4-preferencefragment.svg?branch=master)](https://travis-ci.org/kunny/android-support-v4-preferencefragment)

# PreferenceFragment for support library

Unofficial PreferenceFragment compatibility layer for Android 1.6 and up. 

## How to use

### Install library to local maven repository

Supports install to local maven repository. Simply run `./gradlew install` on the project root. It will install `android-support-v4-preferencefragment` to your local maven repository with following messages :

	$ ./gradlew install
	:compileLint
	:copyReleaseLint UP-TO-DATE
	:mergeReleaseProguardFiles UP-TO-DATE
	:preBuild
	:preReleaseBuild
	:checkReleaseManifest
	:prepareReleaseDependencies
	:compileReleaseAidl UP-TO-DATE
	:compileReleaseRenderscript UP-TO-DATE
	:generateReleaseBuildConfig UP-TO-DATE
	:generateReleaseAssets UP-TO-DATE
	:mergeReleaseAssets UP-TO-DATE
	:generateReleaseResValues UP-TO-DATE
	:generateReleaseResources UP-TO-DATE
	:packageReleaseResources UP-TO-DATE
	:processReleaseManifest UP-TO-DATE
	:processReleaseResources UP-TO-DATE
	:generateReleaseSources UP-TO-DATE
	:compileReleaseJava UP-TO-DATE
	:processReleaseJavaRes UP-TO-DATE
	:packageReleaseJar UP-TO-DATE
	:compileReleaseNdk UP-TO-DATE
	:packageReleaseJniLibs UP-TO-DATE
	:packageReleaseLocalJar UP-TO-DATE
	:packageReleaseRenderscript UP-TO-DATE
	:bundleRelease UP-TO-DATE
	:install

	BUILD SUCCESSFUL

	Total time: 4.864 secs

### Use library from your project

Add following lines on your build.gradle :

build.gradle on project root:

    allprojects {

    	repositories {
            mavenCentral()
            mavenLocal() // Add this line
        }

    }

or if you have just one module on your project, your script will be:

    repositories {
    	mavenCentral()
    	mavenLocal() // Add this line
    }

Next, add the library to your module's dependency :

    dependencies {
    	compile 'com.androidhuman:android-support-v4-preferencefragment:+'
    }

Now you can use `android-support-v4-preferencefragment` on your project.



Origianl credit goes to [kolavar](https://github.com/kolavar).