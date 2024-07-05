Demande d'un certificat WLCG pour les agents CEA / DRF / IRFU
=============================================================

Introduction
------------

Cette documentation détaille la procédure pour obtenir un certificat
TCS [1]_ pour les agents du CEA / DRF / IRFU. Ces certificats sont
délivrés pour pouvoir accéder aux ressources de grilles de calcul,
aux cloud et aux sites Web sécurisés, notamment dans le cadre de
WLCG [2]_.

**Note :** L'utilisateur a la responsabilité d'assurer le séquestre
et la sauvegarde des clés privées des certificats délivrés.


Obtention d'un certificat
-------------------------

Pour obtenir un certificat, il faut suivre les étapes suivantes :

1. Aller à la page : https://cert-manager.com/customer/renater/idp/clientgeant

2. S'identifier avec la fédération d'identités du CEA, en
   choisissant : CEA French Alternatives Energies ans Atomic Energy
   Commission et s'authentifier avec ses identifiants (AB123456 + mobipass)

3. Sélectionner le *Certificate Profile* : "GEANT Personal Authentication"
   et remplir les champs :

   * Enrollment Method: KeyGEneration

   * Key Type: RSA - 2048

   * Mot de passe robuste [3]_

   * Algorithm: AES256-SHA256

4. Le certificat généré est ensuite automatiquement téléchargé sur
   votre ordinateur sous le fichier ``certs.p12``.

Conversion et import
--------------------

Le certificat téléchargé est au format PKCS12. Il peut être chargé
dans le navigateur [4]_ ou transformé au format x509 pour être
utilisé avec les outils de grille de calcul [5]_.


.. [1] Certificat TCS : https://wiki.geant.org/display/TCSNT/TCS+wiki+%282020%29+Sectigo

.. [2] Worldwide LHC Computing Grid : https://wlcg.web.cern.ch/

.. [3] Recommandation de l'ANSSI concernant les mots de passe : https://cyber.gouv.fr/cybermois-2021-les-mots-de-passe

.. [4] Chargement d'un certificat dans le navigateur : https://services.renater.fr/tcs/faq/tcs_personnes/export_import#importer_une_sauvegarde_de_certificat_dans_mon_navigateur

.. [5] Conversion d'un certificat : https://doc.cc.in2p3.fr/fr/Daily-usage/faq/faq-general-help.html#convertir-un-certificat
