# Docker-Django-Nginx-Gunicorn
how to dockerize django project with serve static file by nginx and run over gunicorn



how to use :

# Step-1:

First Copy your project in SRC directory:

# Step-2:
Add STATIC_ROOT = '/HT/static'  to settings file
# Step-3:
Check static file and migrate is Ok in project

# Step-4:

run command :  docker-compose up

Django+ gunucorn run over port 8000 behind of Nginx on port 80
