# Gradle

1. Install required software locally (latest version of Gradle, Java).

2. Go to https://github.com/spring-projects/spring-petclinic, fork it, and clone the forked repo.

3. [Check what tasks are available for the project.](#ad-3)

4. [Run all available project tests.](#ad-4)

5. [Build the project and run it, and verify it’s available on the localhost in the browser.](#ad-5)

6. [Perform the cleanup.](#ad-6)

7. [Explore gradle-related files. Identify which gradle file defines the project name and change it. Build the project again and verify the new project name is being used (you need to find .jar files).](#ad-7)

8. [Create an additional custom task, which depends on the build task (so by calling this task the build and test tasks will also be executed). It should open the browser with generated test results.](#ad-8)

9. [Add the dynamic versioning to your project using the commonly used axion-release-plugin (GitHub - allegro/axion-release-plugin: Gradle release & version management plugin.). Check the Version your project (Gradle best practice tip #5) to find the tutorial on how to do this.](#ad-9)

10. [Check the new available commands after the plugin addition. Using these new commands, check the current project version. Then add and commit some changes to the project and make the project release. Check the current version one more time and git tags available. Note the difference between SNAPSHOT and release versions.](#ad-10)

11. [Perform the cleanup.](#ad-11)


## Ad 3

Checking available tasks for the project:

![Screenshot 2022-11-26 at 13 23 29](https://user-images.githubusercontent.com/114099418/205443742-fed89551-062c-4413-841c-9c1569e18c6f.png)

## Ad 4

Running all available project tests:

![Screenshot 2022-11-26 at 16 45 47](https://user-images.githubusercontent.com/114099418/205443849-1b2f618c-0824-4b4c-b3a9-196998aba18f.png)

## Ad 5

Building the project and running it, and verifying it’s available on the localhost in the browser.

Building:

![Screenshot 2022-11-26 at 16 58 16](https://user-images.githubusercontent.com/114099418/205443923-e0ca8670-6eb3-407d-b1a4-7e7db43c8ab0.png)

Running:

![Screenshot 2022-11-26 at 17 17 37](https://user-images.githubusercontent.com/114099418/205443960-075278a1-0f36-4ee5-ba88-8da19bc3a1f2.png)

Verifying:

![Screenshot 2022-11-26 at 17 17 52](https://user-images.githubusercontent.com/114099418/205443997-5a503267-acc5-4dd2-8fea-d5d733d54480.png)

## Ad-6

Performing the cleanup:

![Screenshot 2022-11-26 at 17 22 22](https://user-images.githubusercontent.com/114099418/205444153-816a4b04-2310-43fa-975d-35fd21c2aa7b.png)

## Ad-7

Exploring gradle-related files. Identifying which gradle file defines the project name and change it. Build the project again and verify the new project name is being used (you need to find .jar files)

Changing project name:

![Screenshot 2022-12-03 at 14 54 32](https://user-images.githubusercontent.com/114099418/205444348-f1c706e8-dd51-4d64-9813-808220312721.png)

Verifying prpject name:

![Screenshot 2022-11-26 at 17 24 17](https://user-images.githubusercontent.com/114099418/205444410-d62e2eaa-4888-427a-ad1d-fd9fa7e97e33.png)

## Ad-8

Creating an additional custom task:

![Screenshot 2022-11-26 at 17 52 06](https://user-images.githubusercontent.com/114099418/205444561-8ac0d783-6b39-4450-ab3c-3fc5c72ed8fe.png)

Verifying that task exist:

![Screenshot 2022-12-03 at 15 12 05](https://user-images.githubusercontent.com/114099418/205445139-26755b9c-df92-4d8b-b915-f63fabb13ff8.png)

Used command:

![Screenshot 2022-12-03 at 15 02 57](https://user-images.githubusercontent.com/114099418/205444825-53248321-5c0b-4342-9ba6-73fb29f9486f.png)

Test results in the browser:

![Screenshot 2022-11-26 at 17 52 51](https://user-images.githubusercontent.com/114099418/205444863-0d5f8f21-ce5d-49cc-ad13-0d06e426addb.png)

## Ad 9

Add the dynamic versioning to your project using the commonly used axion-release-plugin (GitHub - allegro/axion-release-plugin: Gradle release & version management plugin.). Check the Version your project (Gradle best practice tip #5) to find the tutorial on how to do this.

Adding plugin:

![Screenshot 2022-11-26 at 18 00 13](https://user-images.githubusercontent.com/114099418/205444950-a8a84032-3749-4b7e-ad24-98aa77e01d0d.png)

Checking version:

![Screenshot 2022-12-03 at 15 15 32](https://user-images.githubusercontent.com/114099418/205445343-608f41ce-b0c7-4b16-9228-5bea7b2083dd.png)

## Ad 10

Adding and committing some changes to the project:

![Screenshot 2022-12-03 at 15 20 37](https://user-images.githubusercontent.com/114099418/205445541-60ce33f6-ea11-400d-84a8-ba3c178a08fe.png)

 Making the project release:
 
![Screenshot 2022-12-03 at 15 25 59](https://user-images.githubusercontent.com/114099418/205445769-3003c9dc-4a9d-433e-8573-24b578524bea.png)

Checking the current version one more time and git tags available:
![Screenshot 2022-12-03 at 15 27 53](https://user-images.githubusercontent.com/114099418/205445865-f2a52a35-a493-4fe3-af99-f460163c52fa.png)

Differences between SNAPSHOT and release versions:
A "release" is the final build for a version which does not change. A "snapshot" is a build which can be replaced by another build which has the same name. It implies that the build could change at any time and is still under active development. You have different artifacts for different builds based on the same code.

## Ad 11

Performing cleanup:

![Screenshot 2022-12-03 at 15 34 18](https://user-images.githubusercontent.com/114099418/205446260-644d0b2a-b9df-47c3-b52e-d42b310a24ea.png)


