Genghistask.github.io
===================================


https://github.com/GenghisTask/GenghisTask.github.io

The documentation is generated with sphinx https://www.sphinx-doc.org/en/master/

Build the documentation locally with this docker command :

``docker run -v `pwd`:/docs --rm sphinxdoc/sphinx bash -c 'pip install sphinx_rtd_theme && /usr/local/bin/sphinx-build -M html  . _build'``