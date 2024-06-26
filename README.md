# Terminus

Formerly Standard SDK Tests.

This project enables the manual execution, via GitHub Actions, of individual or multiple language SDK tests.

To run the tests do the following:

Click on the Actions tab highlighted below

![image-01](img/image-01.png)

------



Click on Execute Terminus in the left hand panel highlighted below

![image-02](img/image-02.png)

------



On the next screen click on Run workflow.

This will then display a drop down with run options. The Node build repo option defines the branch to build the CCTL Docker image from. If the action cannot locate the Docker image in docker.io then the image will be built by the action runner. Populate the blank language SDK fields with the desired branch to test, leave blank to ignore. See the example below.

![image-03](img/image-03.png)

------



Clicking on Run workflow will present the following screen with the amber badge indicating the action is running

![image-04](img/image-04.png)

------



Clicking on the workflow will present the following screen

![image-05](img/image-05.png)

------



Once the job is completed, success or failure, click on the Summary tab highlighted below

![image-06](img/image-06.png)

------



Scroll down on the next screen and view the run summary as below

![image-07](img/image-08.png)

Click on the artifact file to download the Junit report.

## Notes

We are working within the limitations of GitHub's actions here. For example the dropdown menu can only have ten UI items. We are also using a third party action to display the test summary which has its limitations.

Work will be done to create a Casper specific test summary action in the future.