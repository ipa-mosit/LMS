# LMS
## How to make things work
First thing to do to make things work smoothly is to activate virtual environment.

    source envLMS/bin/activate
As project uses postgresql you should have it installed properly.
Also you need to have a user named osman and a database lms, though all can be changes in settings.py according to your needs. :)
then makemigrations and migrate and after these runserver :)

    python manage.py makemigrations
    python manage.py migrate
    python manage.pyt runserver


