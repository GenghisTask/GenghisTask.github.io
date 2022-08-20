Quickstart
=======================

The easiest way to run the application is this docker command :

``docker run --rm -v /var/run/docker.sock:/var/run/docker.sock  -e GIT_BRANCH=main -e GIT_REPO='https://github.com/GenghisTask/Workspace.git' --network=host  genghistask/ui:2.1.1``

You can use right away the webapp http://127.0.0.1:3000/#/Graphs 

However, it is better at first to discover the additional startup parameters and create you own workspace as discussed in the next page.