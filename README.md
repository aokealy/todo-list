# To do List:
Welcome to my Project four To Do List that I have created which has all the funcitionallity you would expect from a to do list!
- here is a link to my heroku fully deployed app https://todolist-django.herokuapp.com/
- here is a link to my github repository https://github.com/aokealy/todo-list
------------
# User Stories:
-  Agile approach for the user stories which can be found in the project section of the github repository 
- https://github.com/users/aokealy/projects/2

# **User Experience (UX):**
## Wireframes:
The wireframes for the site were created in the software [wirefram cc](https://wireframe.cc/). The wireframes have been created for desktop, tablet and mobile devices. The text content wasn't finalized during the wireframe process. 

- https://wireframe.cc/Iy5cCB - Home Page wireframe layout
- https://wireframe.cc/nrSBdL - Create Task Page layout
- https://wireframe.cc/nrSBdL - Edit Task Page layout
- https://wireframe.cc/TfPn7I - Delete Task Page layout
- https://wireframe.cc/9XduNe - Login Page layout
- https://wireframe.cc/0Wdu9u - Register Account Page layout

# Design Choices:
## Typography:
- Roboto and Pangolin were the google fonts I used for this project.
- Roboto is an open source, sans-serif font originally developed by Google for Android. Its a modern, crisp typeface that pairs well with Archvio, Lora, Rokkit, Nunito, Raleway and Space Mono.
- Pangolin was designed for the Google Valentine's Day 2017 Doodle, Pangolin Love. A pangolin is an endangered species native to Asia and Africa. The font is a sans serif handwriting style. It supports many languages that use the Latin and Cyrillic scripts.

- ![Screenshot](/media/roboto-font.PNG)
- ![Screenshot](/media/pangolin-font.PNG)

## Colour Scheme
- ![#cf4949](https://placehold.co/15x15/cf4949/cf4949.png) `#cf4949`
- ![#FAFAFA](https://placehold.co/15x15/FAFAFA/FAFAFA.png) `#FAFAFA`
- ![#4b5156](https://placehold.co/15x15/4b5156/4b5156.png) `#4b5156`

# Features
## existing features:
- Be able to create users using a registraion system without using admin panel.
- Be able to login into an account and only display your information to protect others
- Be able to logout of your account with ease and not have to use the admin panel
- Be able to  create a task when signed into an account
- Be able to edit a task when signed into an account
- Be able to delete a task when signed into an account
- Be able to check off the task to show completed
- Be able to uncheck the task to mark not completed
- Display if the task is completed or not completed

# Technologies Used
- Python - Provides the functionality for the site.
- HTML5 - Provides the content and structure for the website.
- CSS3 - Provides the styling for the website.
- JavaScript - Provides interactive elements of the website
- Django - A model-view-template framework 
- Heroku - A cloud platform that the application is deployed to.
- Lighthouse - Used to test performance of site.
- HTML Validation - Used to validate HTML code
- CSS Validation - Used to validate CSS code
- JSHint Validation - Used to validate JavaScript code

# Testing:
- Lighthouse score test:
- ![Screenshot](/media/lighouse.PNG)

- HTML Validator:
- ![Screenshot](/media/html-valid.PNG)

- CSS Validator:
- ![Screenshot](/media/css-validator.PNG)



# Reference:

- https://www.youtube.com/watch?v=llbtoQTt4qw&t=3327s&ab_channel=DennisIvy - Dennis Ivy Todo List Inspiration 
- https://cssgradient.io/ - Create colour pallete for back ground colours
- https://www.toptal.com/designers/htmlarrows/symbols/ - This was used for the buttons symbols 
- https://fonts.google.com/ - google fonts for the fonts used in project
- https://wireframe.cc/ - for the wireframes
- https://validator.w3.org/ - html validator
- https://jigsaw.w3.org/css-validator/ - css validator


# Deployment:

## Deployment To Heroku

The project was deployed to [Heroku](https://www.heroku.com). To deploy, please follow the process below:
Use the arrows below to drop down and view the steps

1. To begin with we need to create a GitHub repository from the [Code Institute template](https://github.com/Code-Institute-Org/gitpod-full-template) by following the link and then click 'Use this template'.

<details><summary><b>Heroku Deployment - Step 1</b></summary>

Heroku Deployment Step 1

2. Fill in the needed details as stated in the screenshot below and then click 'Create Repository From Template'.

<details><summary><b>Heroku Deployment - Step 2</b></summary>

![Heroku Deployment Step 2]
</details><br />

3. When the repository creation is done click 'Gitpod' as stated in the screenshot below.

<details><summary><b>Heroku Deployment - Step 3</b></summary>

![Heroku Deployment Step 3]
</details><br />

4. Now it's time to install Django and the supporting libraries that are needed. Type the commands below to do this.

* ```pip3 install 'django<4' gunicorn```
* ```pip3 install 'dj_database_url psycopg2```
* ```pip3 install 'dj3-cloudinary-storage```

<details><summary><b>Heroku Deployment - Step 4</b></summary>

![Heroku Deployment Step 4]
</details><br />

5. When Django and the libraries are installed we need to create a requirements file.

* ```pip3 freeze --local > requirements.txt``` - This will create and add required libraries to requirements.txt

<details><summary><b>Heroku Deployment - Step 5</b></summary>

![Heroku Deployment Step 5]
</details><br />

6. Now it's time to create the project.

* ```django-admin startproject YOUR_PROJECT_NAME .``` - This will create your project

<details><summary><b>Heroku Deployment - Step 6</b></summary>

![Heroku Deployment Step 6]
</details><br />

7. When the project is created we can now create the application.

* ```python3 manage.py startapp APP_NAME``` - This will create your application

<details><summary><b>Heroku Deployment - Step 7</b></summary>

![Heroku Deployment Step 7]
</details><br />

8. We now need to add the application to settings.py

<details><summary><b>Heroku Deployment - Step 8</b></summary>

![Heroku Deployment Step 8]
</details><br />

8. Now it is time to do our first migration and run the server to test that everything works as expected. This is done by writing the commands below.

* ```python3 manage.py migrate``` - This will migrate the changes
* ```python3 manage.py runserver``` - This runs the server. To test it, click the open browser button that will be visible after the command is run.

9. Now it is time to create our application on Heroku, attach a database, prepare our environment and settings.py file and setup the Cloudinary storage for our static and media files.

* Head on to [Heroku](https://www.heroku.com/) and sign in (or create an account if needed).

* In the top right corner there is a button that is labeled 'New'. Click that and then select 'Create new app'.

<details><summary><b>Heroku Step 09</b></summary>

![Heroku Step 9]
</details><br />

10. Now it's time to enter an application name that needs to be unique. When you have chosen the name, choose your region and click 'Create app".

<details><summary><b>Heroku Step 10</b></summary>

![Heroku Step 10]
</details><br />

11. To add a database to the app you need to go to the resources tab ->> add-ons, search for 'Heroku Postgres' and add it.

<details><summary><b>Heroku Step 11</b></summary>

![Heroku Step 11]
![Heroku Step 11]
</details><br />

12. Go to the settings tab and click on the reveal Config Vars button. Copy the text from DATABASE_URL (because we are going to need it in the next step).

<details><summary><b>Heroku Step 12</b></summary>

![Heroku Step 12]
</details><br />

13. Go back to GitPod and create a new env.py in the top level directory. Then add these rows.

* ```import os``` - This imports the os library
* ```os.environ["DATABASE_URL_FROM HEROKU"]``` - This sets the environment variables.
* ```os.environ["SECRET_KEY"]``` - Here you can choose whatever secret key you want.

<details><summary><b>Heroku Step 13</b></summary>

![Heroku Step 13]
</details><br />

14. Now we are going to head back to Heroku to add our secret key to config vars. See screenshot below.

<details><summary><b>Heroku Step 14</b></summary>

![Heroku Step 14]

15. Now we have some preparations to do connected to our environment and settings.py file. In the settings.py, add the following code:

```import os```

```import dj_database_url```

```if os.path.isfile("env.py"):```

```import env```

<details><summary><b>Heroku Step 15</b></summary>

![Heroku Step 15]
</details><br />

16. In the settings file, remove the insecure secret key and replace it with:
```SECRET_KEY = os.environ.get('SECRET_KEY')```

<details><summary><b>Heroku Step 16</b></summary>

![Heroku Step 16]
</details><br />

17. Now we need to comment out the old database setting in the settings.py file (this is because we are going to use the postgres database instead of the sqlite3 database).

<details><summary><b>Heroku Step 17 1/2</b></summary>

![Heroku Step 17]
</details><br />

Now, add the link to the DATABASE_URL that we added to the environment file earlier.

<details><summary><b>Heroku Step 17 2/2</b></summary>

![Heroku Step 17]
</details><br />

18. Save all your fields and migrate the changes.

```python3 manage.py migrate```

19. Now we are going to get our connection to Cloudinary connection working (this is were we will store our static files). First you need to create a Cloudinary account and from the Cloudinary dashboard copy the API Environment Variable.

20. Go back to the env.py file in Gitpod and add the Cloudinary url (it's very important that the url is correct):

```os.environ["CLOUDINARY_URL"] = "cloudinary://************************"```

21. Let's head back to Heroku and add the Cloudinary url in Config Vars. We also need to add a disable collectstatic variable to get our first deployment to Heroku to work.

<details><summary><b>Heroku Step 21</b></summary>

![Heroku Step 21]
</details><br />

22. Let's head back to our settings.py file on Gitpod. We now need to add our Cloudinary Libraries we installed earlier to the installed apps. Here it is important to get the order correct.

<details><summary><b>Heroku Step 22</b></summary>

![Heroku Step 22]

23. For Django to be able to understand how to use and where to store static files we need to add some extra rows to the settings.py file.

<details><summary><b>Heroku Step 23</b></summary>

![Heroku Step 23]
</details><br />

24. Hang in there, we have just a couple of steps left. Now it's time to link the file to the Heroku templates directory.

<details><summary><b>Heroku Step 24</b></summary>

![Heroku Step 24]
</details><br />

25. Let's change the templates directory to TEMPLATES_DIR in the teamplates array.

<details><summary><b>Heroku Step 25</b></summary>

![Heroku Step 25]
</details><br />

26. To be able to get the application to work through Heroku we also need to add our Heroku app and localhost to which hosts that are allowed.

<details><summary><b>Heroku Step 26</b></summary>

![Heroku Step 26]
</details><br />

27. Now we just need to add some files to Gitpod.

* Create 3 folders in the top level directory: **media**, **static**, **templates**
* Create a file called **Procfile* and add the line ```web: gunicorn PROJ_NAME.wsgi?``` to it.d

28. Now you can save all the files and prepare for the first commit and push to Github by writing the lines below.

* ```git add .```
* ```git commit -m "Deployment Commit```
* ```git push```

29. Before moving on to the Heroku deployment we just need to add one more thing in the config vars. We need to add "PORT" in the KEY input field and "8000" in the VALUE field. If we don't add this there might be problems with the deployment.

30. Now it's time for deployment. Scroll to the top of the settings page in Heroku and click the 'Deploy' tab. For deployment method, select 'Github'. Search for the repository name you want to deploy and then click connect.

31. Scroll down to the manual deployment section and click 'Deploy Branch'. Hopefully the deployment is successful!

<details><summary><b>Heroku Step 31</b></summary>

![Heroku Step 31]
</details><br />





## How To Fork The Repository On GitHub

It is possible to do a independent copy of a GitHub Repository by forking the GitHub account. The copy can then be viewed and it is also possible to do changes in the copy without affecting the original repository. To fork the repository, take these steps:

1. After logging in to GitHub, locate the repository. On the top right side of the page there is a 'Fork' button. Click on the button to create a copy of the original repository.

<details><summary><b>Github Fork</b></summary>

![Fork](readme/assets/images/github_fork.png)
</details><br />



## Cloning And Setting Up This Project

To clone and set up this project you need to follow the steps below.

1. When you are in the repository, find the code tab and click it.
2. To the left of the green GitPod button, press the 'code' menu. There you will find a link to the repository. Click on the clipboard icon to copy the URL.
3. Use an IDE and open Git Bash. Change directory to the location where you want the cloned directory to be made.
4. Type 'git clone', and then paste the URL that you copied from GitHub. Press enter and a local clone will be created.

<details><summary><b>Github Create Local Clone</b></summary>

![Clone]
</details><br />

5. To be able to get the project to work you need to install the requirements. This can be done by using the command below:

* ```pip3 install -r requirements.txt``` - This command downloads and install all required dependencies that is stated in the requirements file.

6. The next step is to set up the environment file so that the project knows what variables that needs to be used for it to work. Environment variables are usually hidden due to sensitive information. It's very important that you don't push the env.py file to Github (this can be secured by adding env.py to the .gitignore-file). The variables that are declared in the env.py file needs to be added to the Heroku config vars. Don't forget to do necessary migrations before trying to run the server.

* ```python3 manage.py migrate``` - This will do the necessary migrations.
* ```python3 manage.py runserver``` - If everything i setup correctly the project is now live locally.

<details><summary><b>Setup env.py</b></summary>

![Clone]
</details><br />
----------




