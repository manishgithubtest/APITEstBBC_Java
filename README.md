# APITEstBBC_Java
API Rest assured BDD cucumber page object maven framework on Java (manish)

As part of Submission of my Automation test, the automation task I completed on Java using Page object model on Cucumber BDD. I have divided all five test scenarios in two features files however, created on step Definition class only for both the features.

The project directory contains below:
1. Feature Files (folder path: src/test/resources/features)
• SoundTrackAPI-Scenario1-2. Feature //scenarios 1 & 2
• SoundTrackAPI-Scenario3-4-5. Feature // scenarios 3,4 & 5
2. Runner class " TestRunner_.java” :: Folder path: src/test/java/Runner/
• The runner class is used to run the automation using Junit
3. “Hooks.java” class inside folder: src/test/java/stepDefs/
• This class has the basic code to send the request and extract the response.
4. Step Definition Class “StepDef_MusicTrack.java”: Folder path: src/test/java/stepDefs/
• This is test class corresponding to the feature files, implemented BDD given when then steps.
5. Page class “MusicAPIPg.java” Folder path: src/main/java/APIPages/
• This page folder and the page class created to have a separate java class for each API, this page class has functions/code for the step definition class.
6. “PropertyFileReader.java” class inside folder: src/main/java/utility/
• This class is being used to read the data from property file.
7. “config.properties” file under folder: src/main/resources/
• This file has URL constant, the idea to have separate property file is to segregation of hard code string/constants.
8. “Pom.xml” inside project root directory, contains all maven dependencies.
• Use to build / run and clean project.
• Contains details of all the dependencies.
9. HTML /Json Reports:
• Default cucumber report < APIBBCMSS_TestReport.html > is in folder: target/Reports/
• Customize HTML report with the PIE chart < RegressionTest.html > is in folder: target/ cucumber-report-html / cucumber-html-reports/

Installation/Automation Run Instructions: Assuming that your machine has latest Java/JDK installed and JAVA_HOME path is defined and eclipse is installed.
1. Download the project code folder from the git location that I shared in the email.
2. Unzip the folder
3. If using eclipse then, open the project as exiting maven project
4. Wait for maven dependencies to load completely.
5. Once the dependencies are loaded, select “Pom.xml” file from project explorer section and run the project as “test”.
6. Project execution started , and while the project executing, the details of scenarios can be seen on the console.
7. Once project executed, to see the report, go to
a. Default cucumber report < APIBBCMSS_TestReport.html > is in folder: target/Reports/
b. Customize HTML report with the PIE chart < RegressionTest.html > is in folder: target/ cucumber-report-html / cucumber-html-reports/
8. Additionally, to run the project as JUnit, go to runner class folder in project explorer I.e., Runner class " TestRunner_.java” :: Folder path: src/test/java/Runner/ -> select the runner class and right click on it and select “run as -> Junit”.
9. Once the project execution is completed, the reports can be seen in the same folder as mention before at step number 7
