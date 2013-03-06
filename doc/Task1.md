# Task1: Installation

**What you will need**

1. python2
2. virtualenv

**Installation process**

Make sure your python version is proper

    $ python --version
    Python 2.7.3

If it says 2.7.X, then you can run django. Otherwise install python2. Sometimes the executable is called python2

    $ python2 --version

or

    $ python2.7

If virtualenv has not been created yet, create one

    $ virtualenv ~/app/djangoapp
    $ source ~/app/djangoapp/bin/activate
    (djangoapp)$ 

You should see your command line prefixed with the djangoapp like in the last line above. 

You should clone the repository of kam-tamam. For this

    (djangoapp)$ git clone git@github.com:bibstha/kam-tamam.git
    (djangoapp)$ cd kam-tamam

You are now inside the kam-tamam application. We now install django and the required dependencies.

    (djangoapp)$ pip install -r requirements.txt


