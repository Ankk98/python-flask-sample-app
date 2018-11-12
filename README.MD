## MiniTwit an example application written in Python/Flask

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/b8b007e3257a4ee581e19c9e85903ae0)](https://app.codacy.com/app/Ankk98/python-flask-sample-app?utm_source=github.com&utm_medium=referral&utm_content=Ankk98/python-flask-sample-app&utm_campaign=Badge_Grade_Dashboard)
[![Codefresh build status]( https://g.codefresh.io/api/badges/pipeline/ankk98/Ankk98%2Fpython-flask-sample-app%2Fpython-flask-sample-app?branch=master&key=eyJhbGciOiJIUzI1NiJ9.NWJlM2UzZDdiN2I1ODY1ODM2MTQ2MzEw.9Evl_VjtOLQWMLkev8PT4e7-O2EM4XTYT3IGuA_x_aQ&type=cf-1)]( https://g.codefresh.io/pipelines/python-flask-sample-app/builds?repoOwner=Ankk98&repoName=python-flask-sample-app&serviceName=Ankk98%2Fpython-flask-sample-app&filter=trigger:build~Build;branch:master;pipeline:5be52119f75e176c0b9ed568~python-flask-sample-app)

Original source code from <https://github.com/pallets/flask/tree/16d83d6bb413bec09a656a659b98d897e7abcc81/examples/minitwit>

## Docker instructions

To create a docker image execute: 

`docker build . -t minitwit`

To run the docker image execute:

`docker run -p 5000:5000 minitwit` and visit with your browser <http://localhost:5000>

To run unit tests inside the container execute:

`docker run minitwit python setup.py test`

## Original Readme

MiniTwit 

because writing todo lists is not fun

### What is MiniTwit

A SQLite and Flask powered twitter clone

### How do I use it

1.  Edit the configuration in the minitwit.py file or export an `MINITWIT_SETTINGS` environment variable pointing to a configuration file.

   
2.  install the app from the root of the project directory
   `pip install --editable .`

3.  tell flask about the right application:
   `export FLASK_APP=minitwit`

4.  fire up a shell and run this:
   `flask initdb`

5.  now you can run minitwit:
   `flask run`

The application will greet you on <http://localhost:5000/>.

### Is it tested

You betcha.  Run the `python setup.py test` file to
      see the tests pass.
