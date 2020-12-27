1. Create file called app.yaml. 
  flex means flexible environment, used only for testing
  -b is for binding $PORT port number to the application. The port number is not fixed, it is being decided by GCP itself
  main is the file name, application is the instance name
  instamnces is # of instances. If there are 4 instances & 20 requests come in simultaneously, each instance will receive 5 request

2. Log in to GCP, create new project & open Google Cloud Shell.
    If shell does not start, append cloudshellsafemode=true to URL
  
3. Copy .GIT url of the project from github, run following commands at the cloud shell
  1. git clone <git_url>
  3. gcloud config set project <project_id>
  4. gcloud app deploy
