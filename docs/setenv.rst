===============================
Settting up desktop environment
===============================

Cloning the project
===================

:
	cd c:\projects
	git clone https://github.com/skilledindia/python.git
	cd python

Installing python packages
===========================

Install python3.5 (64bit/32bit based on your desktop operating system)
Packages used are
* `virtualenv`_
* `virtualenvwrapper-win`_
* `ipython`_

:
    set PATH=C:\Python35;C:\Python35\Scripts;%PATH%
    pip3.5 install virtualenv
	pip3.5 install virtualenvwrapper-win
	pip3.5 install ipython notebook
	pip3.5 install sphinx
	lsvirtualenv
	mkvirtualenv skilledindia
	lsvirtualenv
	workon skilledindia
	
	
.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/installation.html
.. _`virtualenvwrapper-win`: https://pypi.python.org/pypi/virtualenvwrapper-win
.. _`ipython`: http://ipython.org/


Sphinx project creation
=========================

:
	mkdir docs
	cd docs
	sphinx-quickstart	
	root = default
	separate src and build dirs: y 
	Name prefix for templates and static dirs: n
	project name: python
	author: jai
	project version: 0.0.1
	src file ext: .rst
	default file: index.rst
	Do you want a epub builder: n
	automatically insert directories from modules: y
	accept other defaults
	create make file: y
	create bat file:y
	

Using Git
=========

Before pushing docs to git:
	cd docs
	make clean
	git add docs
	git commit -am 'adding first documentation'
	git push
	
