.. Genghistask documentation master file, created by
   sphinx-quickstart on Wed Aug 17 17:25:33 2022.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Genghistask's documentation!
=======================================


|ARM Friendly| |M1 Ready| |x64| |amd64|

GenghisTask the task scheduler. 

.. toctree::
   :hidden:
   :maxdepth: 3

   quickstart

.. toctree::
   :glob:
   :maxdepth: 3
   :hidden:
   :caption: Install

   install/*


.. toctree::
   :glob:
   :maxdepth: 3
   :hidden:
   :caption: User Guide

   basic/*

.. toctree::
   :glob:
   :maxdepth: 3
   :hidden:
   :caption: Recipe

   recipe/*

.. toctree::
   :glob:
   :maxdepth: 3
   :hidden:
   :caption: Source code

   developer/*

.. toctree::
   :maxdepth: 3
   :hidden:
   :caption: Links

   Donate <https://www.paypal.com/donate/?cmd=_s-xclick&hosted_button_id=DNXMX4C5MFAZC&source=url>


.. |ARM Friendly| image:: https://img.shields.io/badge/-Pi?style=social&logo=RaspberryPi
.. |M1 Ready| image:: https://img.shields.io/badge/-M1?style=social&logo=apple
.. |x64| image:: https://img.shields.io/badge/-intel?style=social&logo=intel
.. |amd64| image:: https://img.shields.io/badge/-intel?style=social&logo=amd



What is it ?
------------

GenghisTask is an open source, lightweight and secured replacement for
tools such as `Jenkins <https://www.jenkins.io/>`__,
`Visual-tom <https://www.absyss.com/>`__ or `Crontab
UI <https://lifepluslinux.blogspot.com/2015/06/crontab-ui-easy-and-safe-way-to-manage.html>`__.
These tools are already nice CIs or schedulers and in GenghisTask, you
will find again their traditional use case :

* Launch a periodic rsync backup of a folder 
* Manage tasks with an UI, know what’s going on and debug without hassle

.. figure:: ./assets/illustration.png
   :alt: illustration

   

New use cases :

* I need to launch my collection of usefull script on demand unscheduled 
* I need a centralized way to manage the several  crontab and tasks of several server 
* I need rollback, version control and continuous integration of the new tasks 
* I have security concerns and should no be able to inject arbitrary code into a crontab via a web ui  
* I need to launch the task via HTTP as a Hook (or as a Lambda) 
* I need to run a script in any language, even if the scheduler source code is in an other language.





.. list-table:: Featured
   :widths: 25 50

   * - Quickstart
     - .. image:: assets/terminal.png
          :target: quickstart.html