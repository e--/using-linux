git
=================

basic usage
-----------------
::

    git add
    git log
    git status
    git help

remote manager
------------------
::

    git remote -v
    git remote rm origin
    git remote add origin https://github.com/e--/using-linux.git


github password cache
----------------------
::

    git config --global credential.helper cache
    git config --global credential.helper 'cache --timeout=3600' #kepp password in 1 hour

