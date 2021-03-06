## Usefull commands

Install the needed requirements for this project.
````bash
pip install -r requirements.txt
````

Next we need to create and update the local database Django uses internally.
````bash
python manage.py migrate
python manage.py migrate oauth2_provider
````

And that is already all you need to do for setup. So we can now 
start the server locally on port 8000.
````bash
python manage.py runserver 127.0.0.1:8000
````

To register a new client, simply visit: [http://127.0.0.1:8000/o/applications/](http://localhost:8000/o/applications/).

And to test your authorization you can visit [http://django-oauth-toolkit.herokuapp.com/consumer/](http://django-oauth-toolkit.herokuapp.com/consumer/)
to generate a correct link.

There are several advantages of using Django:
* big community
* strong documentation
* plug and play modules available

Advantages of using Django in combination with OAuth plugin:
* several authentication backends already available
    * can be used with OAuth module by design
* simple setup
* maintained module

More in depth documentation about Django in general can be found in the [offical documentation](https://docs.djangoproject.com/en/2.1/).

Special documentation for the OAuth module can be found [here](https://django-oauth-toolkit.readthedocs.io/en/latest/).