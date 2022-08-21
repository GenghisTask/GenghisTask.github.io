Install
=======================

`Fork this project <https://github.com/GenghisTask/Management/fork>`__ to get a workspace of your own, and run :

``docker run  -v /var/run/docker.sock:/var/run/docker.sock  -e GIT_BRANCH=main -e GIT_REPO='ssh://git@github.com/YouGit/Workspace.git' --network=host  genghistask/ui``



.. list-table:: List of parameters
   :widths: 20 20 20
   :header-rows: 1

   * - Argument
     - Description
     - Default
   * - -p 3000:3000 
     - Forward host port towards the port 3000 of the next.js server inside the container
     - 3000
   * - -e GIT_BRANCH=main
     - Git Branch used by the application where your modification will be saved
     - master
   * - -e GIT_REPO=‘ssh://git@github.com/YouGit/Workspace.git’
     -  Git repository where your modifications are fetched or saved
     - https://github.com/GenghisTask/Workspace.git
   * -  -v /var/run/docker.sock:/var/run/docker.sock
     - Share docker socket to allow launch containers
     - only required if you want to launch job with docker
   * - ``--network=host``
     - Forward all host port 
     - not required
   * - ``--rm``
     - Delete all unsaved modification when the container will be stopped unless -v is used below
     - not required
   * - -v ```pwd```/workspace/:/app/data/api
     - Edit the workspace directly from the host 
     - not required
   * - -v ```pwd```/ssh/ :/root/.ssh
     - Share ssh identity from the host
     - not required but usefull to preserve key accross update
   * - -v ```pwd```/credentials.json :/app/credentials.json
     - Override the credentials file to specify a relational database
     - not required, data goes in plain text if not configured
   * - genghistask/ui
     - This docker image
     - latest

It is better to change GIT_REPO url to match your fork, for example :
GIT_REPO=‘ssh://git@github.com/YouGit/Workspace.git’

You can now use the webapp at http://127.0.0.1:3000/#/Graphs and read the next page to configure the application.