# URL-Shortner Application Deployment
## About The Project
<img width="1434" alt="Screen Shot 2023-08-27 at 7 44 41 PM" src="https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/750667a7-0257-4165-a193-60ec6dc0545e">

In this project, the application - URL-Shortner-Deployment is built and tested with Jenkins. After successful test in Jenkins, the application is 
then deployed using AWS Elastic Benstalk.
** Project Plan

## Technologies Used
* CI/CD Pipeline
** GitHub - commited the application files to a Github Repository
** AWS EC2
** AWS Beanstalk
** Jenkins
* Programming Languages for the Url-Shortner-Application
** Html
** CSS
** JSON
** Flask
** Popper.js
** Bootstrap

## Recreate The Project
* Step 1
** Create an Instance on AWS
*** Use the Ubuntu OS
*** Be sure to use ports 80, 8080, 22
https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/13de008b-d2bb-43e5-9bb7-bba16d6c510d
*** Run the command - Sudo Apt Update - to update your instance
*** Run the command - Sudo Apt Install openjdk-17-jre - to install JDK
*** Click here to install Jenkins: https://www.jenkins.io/doc/book/installing/linux/#debianubuntu
*** Go to your browser and type in yourinstancepublicIPAddress:8080
<img width="1218" alt="Screen Shot 2023-08-28 at 11 52 52 AM" src="https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/c3611a31-7be9-4a32-a69b-bcf42d957b3c">

*** Run the command - sudo cat /var/lib/jenkins/secrets/initialAdminPassword - to grab your admin password
*** Paste your admin password in the Jenkins Application on your browser
** On the Jenkins Application
*** Create your ci/cd pipeline
<img width="950" alt="Screen Shot 2023-08-28 at 12 04 17 PM" src="https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/02aed8fa-a85c-4c14-8d82-8ea5d0d8b148">
*** Fork this code to your own GitHub Repository - code located here: https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/13de008b-d2bb-43e5-9bb7-bba16d6c510d
*** Grab your URL From your Github Repository
<img width="936" alt="Screen Shot 2023-08-28 at 12 09 28 PM" src="https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/388010ec-68de-4795-beae-a1979864c53a">
*** Paste this URL in Jenkins
<img width="1090" alt="Screen Shot 2023-08-28 at 12 12 03 PM" src="https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/8de66420-bf80-463c-b367-7c812e886c61">
*** Don't forget to generate a token on Jenkins
** Observe your pipeline
<img width="1085" alt="Screen Shot 2023-08-27 at 12 21 52 AM" src="https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/807e7d66-01ca-4050-beba-f12f8fb738bc">
*** jenkins will package the files in a zipfile. You will see the pipeline pause. Go ahead and resume.
*** If your pipeline is successfully built and tested like the image below, you can deploy your files using AWS Beanstalk
<img width="1100" alt="Screen Shot 2023-08-27 at 12 22 12 AM" src="https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/0404c09e-bd70-4867-9866-00f2e1073b0c">
*** Download and zip your files from GitHub. This is important because Beanstalk can only accept a zip file.
** On AWS Beanstalk
*** Create Your IAM Roles
<img width="324" alt="Screen Shot 2023-08-28 at 12 37 16 PM" src="https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/ed973c07-2b42-43de-94e2-d5686df8856d">
*** Create Your Beanstalk Deployment
<img width="1281" alt="Screen Shot 2023-08-28 at 12 36 30 PM" src="https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/f0138785-4060-4d9c-9212-e1085f2722a4">
*** Upload your zip file to Beanstalk
*** Check the health status. The goal is to get an ok health status like below.
<img width="1123" alt="Screen Shot 2023-08-27 at 7 44 28 PM" src="https://github.com/DarrielleEvans/URL-Shortner-Deployment/assets/89504317/182a0fff-fcc6-42cc-b3bd-df39b70cfc23">
** click the domain name to see your application deployed





  


  

  


