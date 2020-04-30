# multi-docker-container-project

This is a multi container react application. For multi container application we Elastic bean stalk have many docker file, which file i need to run or build kind things.So we need some kind of configure everything in a file Dockerrun.aws.json. 
Here i have deployed it into Amazon Elastic Beanstak..
Here i have 4 containers in this application so for deploying purpose we need to write some task definition to the Dockerrun.aws.json file.
If you want any documentation regarding task definition for containers then just checkout amazon serveices officaial site by just search on google like "Amazon elastic containers services task definition" and go to Task Definition -> Container definition.




Download the ZIP file from the Releases section of this repository.
Login to the Elastic Beanstalk Management Console
Click 'Create New Application' and give your app a name and description
Click 'Create web server' and select an IAM instance profile to use.
Note: Please ensure the IAM instance profile you select has the necessary permissions. For more information, see Container Instance Role
Choose 'Multi-container Docker' in the 'Predefined configuration' dropdown and click Next
Upload the ZIP file downloaded in step 1
Review and launch the application
