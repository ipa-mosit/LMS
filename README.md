# LMS
## How to make things work
First thing to do to make things work smoothly is to create and activate a virtual environment.

    python -m venv envLMS
    source envLMS/bin/activate

Then you should need to install required packages into this virtual environment by executing the command:

    pip install -r requirements.txt

As project uses postgresql you should have it installed properly.
Also you need to have a user named osman and a database lms, though all can be changes in settings.py according to your needs. :)
then makemigrations and migrate and after these runserver :)

    python manage.py makemigrations
    python manage.py migrate
    python manage.pyt runserver


