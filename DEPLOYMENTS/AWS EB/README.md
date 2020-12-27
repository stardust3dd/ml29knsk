1. EB is designed for developing web applications with Web-API.
2. In EC2, we have to configure manually each & every aspect of the virtual server machine. In EB, it is already provided.

1. Your main python file name should be application.py
2. Your flask object name, which we have defined in application.py should also be the application.
3. .ebignore  is responsible to hold the name of those files which we don't want to push on a cloud.
4. Create a requirements.txt file.
        Command : pip freeze > requirements.txt
5. Create a folder called .ebextensions, for elasticbeanstalk extensions
6. Inside .ebextensions create a python.config file.
7. Mention the commands in python.config
            // option_settings:
              // "aws:elasticbeanstalk:container:python":
                // WSGIPath: application:application

   Inside elasticbeans AWS, look for a python container, application is the driver file
 8. ZIP everything. We have to upload the ZIP later.

8. Create new web app at https://console.aws.amazon.com/elasticbeanstalk/home?region=us-east-1#/welcome
9. Tags not needed. Select Python as platform.
10. Click on Create application, fill out the fields & upload the ZIP. EB will automatically configure the S3 bucket & launch the app

11. App available at http://liremd-env.eba-bnppqumi.us-east-1.elasticbeanstalk.com/predict

