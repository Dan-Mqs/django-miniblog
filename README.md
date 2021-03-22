# django-miniblog
 First working app using Django


## How to run locally for testing

Clone the project into your computer:
```
git clone https://github.com/Dan-Mqs/django-miniblog.git
```

Create and start a virtual environment:
```
py -m venv /path/to/new/virtual/environment
cd <path to you venv>/scripts
activate
```

Install the project dependencies:
```
pip install -r requirements.txt
```

Create a file named "keyfile.py" in the folder "Miniblog_project/Miniblog_Project/"

In "keyfile.py" write the following code (set <your_key> value to any string to use as a key):
```
key_string = '<your_key>'
```

Run: 
```
py manage.py migrate
```

Create admin account:
```
python manage.py createsuperuser
```

Then run:
```
python manage.py makemigrations posts
```

Then run again:
```
python manage.py migrate
```

Start the development server:
```
python manage.py runserver
```

Open the page in your browser to view the app running in the address:
http://localhost:8000/posts/
or
http://localhost:8000/admin/
(Note: use "admin" page to add posts to the blog)
