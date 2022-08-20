
Run a task remotely
=======================

By default, all task are run locally, but is is possible to specify a
remote environment where the task should be executed.



Run through a ssh connection
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

It is possible to define a ssh host where a task can be executed.

You cannot define an ssh remote within the task scheduler directly. 1/
For safety reason, you need to edit the ssh/config file first in the
environment folder of the git repository. 2/ Pull the config file into
the application, using the “Restore” button 3/ The ssh remote should now
be listed as environment. 4/ Remember to also add the public ssh key of
the app to the ssh server.

Run a task inside a docker container
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

It is possible to define an docker container image where a task can be
executed.

You cannot define a docker image within the task scheduler directly. 1/
For safety reason, you need to add the image as service in the
docker-compose file first in the git repository 2/ Pull the config file
into the application, using the “Restore” button 3/ The docker image
should now be listed as environment.
