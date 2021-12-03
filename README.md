# Flask

STEP 1
from flask import Flask

// This line I import Flask class. An instance of this class will be our WSGI application.
//The Web Server Gateway Interface is a simple calling convention for web servers to forward requests to web applications or frameworks written in the Python programming language.


STEP2

//We create an instance of our class. 
__name__ is convenient and appropriate in most cases. 
app = Flask(__name__)
This is needed so that Flask knows where to look for resources such as templates and static files.

STEP 3
We then use the route() decorator to tell FLask what URL should trigger our function

@app.route("/")

STEP4
The function returns the message we want to display in the user's browser. The default is of the content type HTML

NB: The file should not be named flask.py cause it would conflict with Flask itself. Give it either hello.py or something else
