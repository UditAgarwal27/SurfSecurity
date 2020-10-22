# SurfSecurity
Security system to prevent Shoulder Surfing Attacks.

REQUIREMENTS:
<li> Python 3.6+ </li>
<li> XAMPP INSTALLED </li>

METHOD TO CONFIGURE PROJECT:
1. Clone the repo to a root folder. (eg. SSP)
2. Extract the repo to root directory.
3. Go to directory SurfSecurity-master , just created.
4. Move all the folders and file to root folder(SSP)
5. Delete SurfSecurity-master (as ir is empty)
6. Open Command Prompt
7. CD TO root folder(SSP)
8 Enter the following commands -->
  8.1 pip install virtualenv
  8.2 virtualenv ssp_env
  8.3 ssp_env\Scripts\activate
--> Virtual environment is created and run.
  8.4 pip install requirements.txt
(do not close command prompt)

CREATING THE DATABASE REQUIRED:
1. Open the XAMPP controller.
2. Start the Apache and MySQL server. (KEEP THEM OPEN)
3. Open Browser and go to localhost/phpmyadmin
4. Create a databae named "ssp". Create no table in it.
5. Go to root folder(SSP). Go to Register Folder. Fo to LogicFiles Folder. Open "connectToDatabase.py" in a text editor (preferable IDLE).
6. Uncomment the commentd part (the SQL query and cursor.execute). Run the file.
7. Once file is run, again comment the both part (the SQL query and cursor.execute). Save the file and close it.

RUN THE PROJECT
1. Open the command project. (Virtual environment should be running and the curent folder open should be root folder(ssp))
2. Run the following commands -->
  2.1 python manage.py makemigrations
  2.2 python manage.py migrate
  2.3 python manage.py runserver
3. Open browser and enter the url --> localhost:8000/login

<<- THIS IS ONLY DEMO. CERTAIN VERIFICATION AND AUTHENTICATION SCEHEMES ARE STILL NEEDED TO BE DONE -->
 
