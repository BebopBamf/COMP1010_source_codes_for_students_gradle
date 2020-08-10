# COMP1010 2020 Session 2 Source Codes for Students Gradle Project

This is a gradle port of the 2020 session 2 source codes for students

## Common commands and usage

cd into target directory to run tests

e.g.

`$ ~/COMP1010_source_codes_for_students_gradle cd practicePackage`

run gradle

On Windows

`.\gradlew.bat command`

On Unix/Mac/Linux

`./gradlew command`

Build javadocs

`./gradlew javadoc`

Run all unit tests

`./gradlew test -i`

Run certain tests

`./gradlew test --tests packagename.classname.testmethodname -i`

To clean build files

`./gradlew clean`


note: -i provides more useful information when running tests but is not necessary
note2: must be in right directory to use gradle project, e.g. to test practicePackage code must be in practicePacakge directory
note3: replace test with cleanTest to run clean build files before running tests

## Examples

To run introduction/Stage1/testSquare()

`./gradlew test --tests practicePackage.introduction.testsAttempts.Stage1Test.testSquare -i`

To run lists/customBuiltLists/customArrayList/testsAttempts/CustomArrayListTest/testGrow()

`./gradlew test --tests practicePackage.lists.customBuiltLists.customArrayList.testsAttempts.CustomArrayListTest.testGrow -i`
