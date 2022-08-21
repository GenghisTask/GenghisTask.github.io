
Run a task remotely
=======================

By default, all task are run locally, but is is possible to specify a
remote environment where the task should be executed.



Through a ssh connection
************************

It is possible to define a ssh host where a task can be executed.

You cannot define an ssh remote within the task scheduler directly. 

Edit the env file
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
For safety reason, you need to edit the ssh/config file first in the environment folder of the git repository. 

Pull the file
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Pull the config file into the application, using the Pull button 

Find the new env
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The ssh remote should now be listed as environment. 

Configure server
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Remember to also add the public ssh key of the app to this ssh server.

Inside a docker container
************************

It is possible to define an docker container image where a task can be
executed.

You cannot define a docker image within the task scheduler directly. 

Edit the env file
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
For safety reason, you need to add the image as service in the docker-compose file first in the git repository 


Pull the file
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Import the config file into the application, using the Pull button 


Find the new env
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The docker image should now be listed as environment.


Kubernetes
************************

Edit the env file
~~~~~~~~~~
Create a manifests file in the ./environment/kubectl/ directory