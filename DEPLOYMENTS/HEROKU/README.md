Point 1. Your main python file name should be app.py
Point 2. Your flask object name, which we have defined in app.py should also be the app.

Step1: Create a new anaconda environment
        -- conda create -n linearapp python==3.6.9
        
Step2: Install the requirements file
        -- pip install -r requirements.txt
        
Step3: Create a file name as Procfile
        There is no extension for this Procfile
        P should be capital
        -- CONTENT: web: gunicorn app:app
        First app is file name, second app is name of the flask object
        
Step4: Initialise your project as git project
       -- git init
       
Step5: Start tracking all the project files
        -- git add .
        -- git commit -m "First commit"
        -- git status // track all files that are not up to date within git
        
Step6: Build on Heroku
       -- heroku create <app_name> // create the app
       -- git push heroku master // push the local app to heroku clouds
       
THIS APP IS DEPLOYED AT https://liremd.herokuapp.com
THIS APP CAN BE FOUND AT 
