## Starting from the Terminal

In case you want to run your Django application from the terminal just run:

1) Run syncdb command to sync models to database and create Django's default superuser and auth system

    $ python manage.py migrate

2) Run Django

    $ python manage.py runserver $IP:$PORT
    
from courses.models import Course
c = Course()
c.title = "Python Basics"
c.description = "Learn the basics of Python"
c.save()

Course.objects.all()

Course(title="Python Collections", description="Learn about list, dict, and tuple"
   ...: ).save()
Course.objects.create(title="Object-Oriented Python", description="Learn about Python's classes")

git add -A && git commit -m "first commit" && git push -u origin master