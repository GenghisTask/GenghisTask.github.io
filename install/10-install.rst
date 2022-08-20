Install
=======================

`Fork this project 
 <https://github.com/GenghisTask/Management/fork>`__ to get a workspace of your own and run :

``docker run  -v /var/run/docker.sock:/var/run/docker.sock  -e GIT_BRANCH=main -e GIT_REPO='ssh://git@github.com/YouGit/Workspace.git' --network=host  genghistask/ui:2.1.1``

+--------------------+-------------------------------+----------------+
| Argument           | Description                   | Default        |
+====================+===============================+================+
| -p 3000:3000       | Forward host port towards the | 3000           |
|                    | port 3000 of the next.js      |                |
|                    | server inside the container   |                |
+--------------------+-------------------------------+----------------+
| -e GIT_BRANCH=main | Git Branch used by the        | master         |
|                    | application where your        |                |
|                    | modification will be saved    |                |
+--------------------+-------------------------------+----------------+
| -e                 | Git repository where your     | https://github |
| GIT_REPO=‘ssh://gi | modifications are fetched or  | .com/GenghisTa |
| t@github.com/YouGi | saved                         | sk/Workspace.g |
| t/Workspace.git’   |                               | it             |
+--------------------+-------------------------------+----------------+
| –network=host      | Forward all host port         | not required   |
+--------------------+-------------------------------+----------------+
| –rm                | Delete all unsaved            | not required   |
|                    | modification when the         |                |
|                    | container will be stopped     |                |
+--------------------+-------------------------------+----------------+
| -v                 | Edit the workspace directly   | not required   |
| ``pwd``/workspace/ | from the host                 |                |
| :/app/data/api     |                               |                |
+--------------------+-------------------------------+----------------+
| genghistask/ui:2.1 | This docker image             | latest         |
| .1                 |                               |                |
+--------------------+-------------------------------+----------------+

It is better to change GIT_REPO url to match your fork, for example :
GIT_REPO=‘ssh://git@github.com/YouGit/Workspace.git’

You can now use the webapp at http://127.0.0.1:3000/#/Graphs and read the next page to configure the application.