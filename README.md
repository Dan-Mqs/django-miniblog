# django-miniblog
 First working app using Django


## How to run locally for testing

Clone the project into your computer:
```
git clone https://github.com/Dan-Mqs/django-miniblog.git

```

Create and start a a virtual environment:
```
virtualenv env --no-site-packages
source env/bin/activate
```

Install the project dependencies:
```
pip install -r requirements.txt
```

Create a file named "keyfile.py" in the folder "Miniblog_project/Miniblog_Project/"

In "keyfile.py" write the code - set <your_key> value to any string to use as a key:
```
key_string = '<your_key>'
```

Run: 
```
python manage.py migrate
```

Create admin account:
```
python manage.py createsuperuser
```

Then run:
```
python manage.py makemigrations posts
```

Then run
```
python manage.py migrate
```

Start the development server:
```
python manage.py runserver
```

Open localhost:8000 in your browser to view the app running.
