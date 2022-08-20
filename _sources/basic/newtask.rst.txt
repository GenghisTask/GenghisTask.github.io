
Create your own task
=======================

You cannot inject code within the task scheduler directly (if you can,
please file an issue, you discovered a vulnerability, congratulation).

1/ For safety reason, you need to commit here, in the shell folder, a
script first. If the remote git repository is a Github, Gitlab, Gogs or
Gitea it should be easy to add some new file with their web editor. 2/
Pull the script into the application, using the “Restore” button 3/ The
script file should now be listed when you will create or update a job.