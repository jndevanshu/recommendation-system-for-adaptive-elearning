Recommendation-System-for-Adaptive-E-Learning
=============================================

Recommendation System for Adaptive E-Learning



Create a database in mysql with the name elearning_reco_db. grant permissions to the desired user and password. change the settings accordingly in settings.py ddatabase. Django framework provides its own wsgi server for testing the
application in local machine before it is hosted. Following steps must be followed to
start an application :
1. Change the directory to the project directory

2. Run the celery server first (so that work can be performed using worker nodes)
using the following command :

	celery −A elearningsite worker −l info

The terminal will show message on successful deployment of celery worker node.
All the messages related to the backend tasks running on celery can be viewed
on this terminal

3. A new terminal is opened. Now the server has to started using the following
command :

	python manage.py runserver

This will run the server on the same local machine. Appropriate message is
displayed on successful deployment of local server along with the port number
on which the server is running. All the request made to the server and all the
responses sent can be easily monitored via this terminal

4. Open a browser and visit localhost or 127.0.0.1. This will take the user to the
login page.