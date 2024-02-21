Documentation
=============

Ce dépôt contient les documentations France Grilles au format
reStructuredText.

Génération des fichiers PDF
---------------------------

La génération des fichiers PDF est réalisée avec la commande
**pandoc** :

.. code-block:: console

   $ pandoc -V papersize=a4 -V colorlinks=true -V linkcolor=blue -V urlcolor=red -V toccolor=gray \
   > -V margin-top=1in -V margin-left=1in -V margin-right=1in -V margin-bottom=1in \
   > -o documentation.pdf documentation.rst

Documentations complémentaires
------------------------------

* Format reStructuredText : https://docutils.sourceforge.io/rst.html

* Documentation sur le format rst dans Sphinx : https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html
