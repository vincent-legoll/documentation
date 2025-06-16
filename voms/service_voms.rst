Service VOMS France Grilles
===========================

Introduction
------------

L'accès à l'infrastructure de grille de calcul et aux ressources
France Grilles repose sur l'utilisation d'un service VOMS, que ce soit
pour l'authentification ou les autorisations.

Cette documentation détaille la configuration d'un client VOMS pour
pouvoir utiliser s'authentifier auprès du service VOMS de la VO
``vo.france-grilles.fr``.


Service VOMS
------------

Le service VOMS est hébergé par `IJCLab <https://www.ijclab.in2p3.fr/>`_
et se dénomme ``voms-fg.ijclab.in2p3.fr``.


Configuration
-------------

La configuration du client VOMS pour la VO ``vo.france-grilles.fr`` repose sur deux fichiers :

1. Le ficher LSC ``/etc/grid-security/vomsdir/vo.france-grilles.fr/voms-fg.ijclab.in2p3.fr.lsc`` [1]_,
   ayant pour contenu :

   .. code-block::

      /DC=org/DC=terena/DC=tcs/C=FR/L=Paris/O=Centre national de la recherche scientifique/CN=voms-fg.ijclab.in2p3.fr
      /C=GR/O=Hellenic Academic and Research Institutions CA/CN=GEANT TLS RSA 1


2. Le fichier VOMSES ``/etc/vomses/vo.france-grilles.fr-voms-fg.ijclab.in2p3.fr`` [2]_,
   dont le contenu est :

   .. code-block::

      "vo.france-grilles.fr" "voms-fg.ijclab.in2p3.fr" "443" "/DC=org/DC=terena/DC=tcs/C=FR/L=Paris/O=Centre national de la recherche scientifique/CN=voms-fg.ijclab.in2p3.fr" "vo.france-grilles.fr"


Documentation externe
---------------------

1. Guide d'installation d'un client VOMS : https://italiangrid.github.io/voms/documentation/voms-clients-guide


.. [1] `<./voms-fg.ijclab.in2p3.fr.lsc>`_

.. [2] `<./vo.france-grilles.fr-voms-fg.ijclab.in2p3.fr>`_