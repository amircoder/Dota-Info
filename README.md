# Work in progress
Multi-module demo app that gets data from dota2 api.

# Demo
<div style="width: 45%">
    ![App Demo1](art/demo1.gif)
</div>
<div style="width: 45%">
    ![App Demo2](art/demo2.gif)
</div>


# App Design (Likely to change)

### Module 1 (app)
Type: android application.

MainActivity, BaseApplication, Theme.

### Module 2 (core)
Type: java/kotlin library.

Core business models and classes.

### Module 3 (hero)
Type: java/kotlin libraries.

Contains 3 sub-modules:
1. hero-datasource
    - Contains the datasources (network and cache) for the hero Module.
1. hero-domain
    - domain models and classes for the hero Module.
1. hero-interactors
    - Use-cases for the hero Module.

### Module 4 (ui-heroList)
Type: android-library.

UI components for the HeroList screen.

### Module 5 (ui-heroDetail)
Type: android-library.

UI components for the HeroDetail screen.


# build.gradle files
There are 3 types of build.gradle files.
1. android application (app module)
1. android-library-build.gradle
    - Android module that contains ui components.
1. library-build.gradle
    - Pure java/kotlin library.


# API
https://docs.opendota.com/

### Hero Stats (GET)
https://api.opendota.com/api/heroStats

# Known issues
1. [HeroListFilter.kt]()
    - Changing the filter does not rebuild the dialog with the correct size.


# Credits
1. [Hristijan](https://twitter.com/funky_muse)
    - Thanks for the chat and great [sample](https://github.com/FunkyMuse/Aurora).

















