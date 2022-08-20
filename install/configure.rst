Configure
===================================

You can use right away the webapp http://127.0.0.1:3000/#/Graphs, but
it’s best to configure it properly (mainly create a ssh key pair) to be
able to save your modifications. If you do not fork and change GIT_REPO
url to match your fork like
GIT_REPO=‘ssh://git@github.com/YouGit/Management.git’ you may not be
able to save your modifications, tasks, schedule, etc…

If you start the application for the first time, the webapp
http://127.0.0.1:3000/#/Graphs reveals three tasks. You can run the task
in order to configure the application if you don’t want to do it
manually. 1/ You need to create a ssh key pair for the app. Run the
first task (start arrow on the graph) to generate a key. Retrieve the
public key from the stdout log file and add it to the remote git
repository fork. 2/ Check if the remote git repository url is well
configured and if it accepts the key. Run the second task. Control the
STDERR file for this second task. 3/ Override this first time
configuration with the content of the remote git repository, run the
third task.

Now, you can create your own tasks :ref:`./basic/newtask` and your own environnements :ref:`./basic/remotely` 