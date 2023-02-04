Forage - Solution Code
==================================

Solution code for the fifth independent project for Android Basics in Kotlin. This project pairs
with Unit 5 of Android Basics in Kotlin

Introduction
------------

This is my solution code for the Forage app project. This project is an opportunity for me to
demonstrate the concepts I learned in Unit 5 of Android Basics in Kotlin.

Pre-requisites
--------------

- Complete Unit 1 of Android Basics in Kotlin
- Complete Project 1: Lemonade App
- Complete Unit 2 of Android Basics in Kotlin
- Complete Project 2: Dogglers
- Complete Unit 3 of Android Basics in Kotlin
- Complete Project 3: Lunch Tray
- Complete Unit 4 of Android Basics in Kotlin
- Complete Project 4: Amphibians
- Complete Unit 5 of Android Basics in Kotlin

Getting Started
---------------

1. Download the starter code
2. Open the project in Android Studio
3. Complete the project in accordance with the app requirements


Tasks
---------------

Tips
----

- Use the provided tests to ensure your app is running as expected
- DO NOT ALTER THE PROVIDED TESTS

----------------- My observations:
If you want to view the SQLite database use View -> Tool Window -> App Inspection (Database Inspector)

The SQLite database name is forageable_database, you can export it by right clicking and -> Export As File...

Although the app works fine, I haven't been able to run any tests. The message that appears is:
Launching 'PersistenceInstrumentationTests' on Pixel API 31.
Install successfully finished in 4 s 268 ms.
Running tests

$ adb shell CLASSPATH=$(pm path androidx.test.services) app_process / androidx.test.services.shellexecutor.ShellMain am instrument -r -w -e targetInstrumentation com.example.forage.test/androidx.test.runner.AndroidJUnitRunner    -e debug false -e class 'com.example.forage.PersistenceInstrumentationTests' androidx.test.orchestrator/androidx.test.orchestrator.AndroidTestOrchestrator
"Run Android instrumented tests using Gradle" option was ignored because this module type is not supported yet.

Googling for solutions, I discovered:

https://stackoverflow.com/questions/71513360/run-android-instrumented-tests-fail/71864048#71864048

which however does not work.
