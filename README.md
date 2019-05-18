# LMS
## How to make things work
First of all you need to clone the project to somewhere in your drive by executing the command:

    git clone https://github.com/ipa-mosit/LMS.git

Second thing to do to make things work smoothly is to create and activate a virtual environment.
Note:As i use archlinux, it is enough for me to type python, you may need to type in "python3" instead.

    python -m venv envLMS
    source envLMS/bin/activate

Note2: whenever want to deactivate the virtual environment just type "deactivate" and press enter. But don`t do that right now :)

Then you should need to install required packages into this virtual environment by executing the command:

    sudo pip install -r requirements.txt

As project uses postgresql you should have it installed properly.
Also you need to have a user named osman and a database lms, though all can be changes in settings.py according to your needs. :)
then makemigrations and migrate and after these runserver :)

    python manage.py makemigrations
    python manage.py migrate
    python manage.pyt runserver

Now server is activated and you may reach the greeting page from the address: "http://localhost:8000/" 
Though, you need to create at least a user to login. To do so close the server and type the following command from bash:

    python manage.py createsuperuser

