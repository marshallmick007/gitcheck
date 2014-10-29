gitcheck
========

If you working in multiples projects, you want can be analyzed in a
single pass of the changes in your projects. gitcheck is script who scan
recursive directory to find a git directory and analyse all
modifications.

Installation
------------

::

    pip install git+git://github.com/marshallmick007/gitcheck.git

Examples utilizations
---------------------

Simple version
~~~~~~~~~~~~~~

In simple version, it show for each repositories if you have
modification not committed and or commits not pushed.

.. code:: bash

    > gitcheck.py

.. figure:: http://bruno.adele.im/static/gitcheck.png
   :alt: Gitcheck simple

   Gitcheck simple

Verbose version
~~~~~~~~~~~~~~~

Substantially identical to the previous version, in bonus, it print who
files modified and commits not pushed

.. code:: bash

    > gitcheck.py -v 

.. figure:: http://bruno.adele.im/static/gitcheck_verbose.png
   :alt: Gitcheck verbose

   Gitcheck verbose

Options
~~~~~~~

.. code:: plaintext

    -v, --verbose                     Show files & commits
    -r, --remote                      also check with the remote
    -b, --bell                        bell on action needed
    -w <sec>, --watch <sec>           after displaying, wait <sec> and run again
    -i <re>, --ignore-branch <re>     ignore branches matching the regex <re>
    -d <dir>, --dir                   Search <dir> for repositories

French version is available here
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

http://bruno.adele.im/projets/gitcheck/
