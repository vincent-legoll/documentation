Demande d'un certificat personnel IGTF
======================================

Introduction
------------

Cette documentation détaille la procédure pour obtenir un certificat
TCS [1]_ pour les agents du CNRS. Ces certificats sont notamment
délivrés pour pouvoir accéder aux ressources de grilles de calcul,
aux cloud et aux sites Web sécurisés.

Pour ceux qui souhaitent avoir plus d'information concernant les
certificats, RENATER maintient une documentation à jour [2]_.

**Important :** L'utilisateur a la responsabilité d'assurer le séquestre
et la sauvegarde des clés privées des certificats délivrés.


Obtention d'un certificat
-------------------------

L'obtention d'un certificat n'est possible que pour les agents ayant un
identifiant d'un établissement public de l'Enseignement Supérieur et
de la Recherche.

Pour obtenir un certificat, il faut suivre les étapes suivantes :

1. Se rendre sur le portail HARICA : https://cm.harica.gr/

2. Se connecter en utilisant le bouton "Academic Login"

3. S'identifier à l'aide de vos identifiants CNRS. Pour cela, il faut
   sélectionner "CNRS - Personnels des unités" et passer à l'étape
   suivante. Il vous est alors demandé de vous identifier avec vos
   identifiants Janus.

4. Sélectionner un certificat IGTF en cliquant sur "IGTF Client Auth" dans
   le menu de gauche puis cliquez sur "Next"

5. Cocher la case d'acceptation des conditions d'utilisation, après les
   avoir lues et cliquez sur "Submit Request".

6. Sur l'écran suivant, cliquez sur "Enroll your Certificate"

7. Laissez les valeurs par défaut, entrez un mot de passe robuste [3]_, cochez
   comme quoi vous comprenez que seul vous connaissez votre mot de passe.
   Cliquez sur "Enroll Certificate"

8. Cliquez sur "Download" pour télécharger votre certificate. Notez que
   c'est le seul moment où vous pourrez télécharger votre certificat.
   Le fichier est téléchargé sous le nom "Certificate.p12".


En cas de problème
------------------

Si vous rencontrez des difficultés dans la génération de votre
certificat, vous pouvez contacter l'assistance du site SESAME en
cliquant sur le lien "Assistance" en bas à droite.

Conversion et import
--------------------

Le certificat téléchargé est au format PKCS12. Il peut être chargé
dans le navigateur [4]_ ou transformé au format x509 pour être
utilisé avec les outils de grille de calcul [5]_.


.. [1] Certificat TCS : https://wiki.geant.org/display/TCSNT/TCS+wiki+%282020%29+Sectigo

.. [2] Documentation RENATER sur les certificats : https://services.renater.fr/tcs/index

.. [3] Recommandation de l'ANSSI concernant les mots de passe : https://cyber.gouv.fr/cybermois-2021-les-mots-de-passe

.. [4] Chargement d'un certificat dans le navigateur : https://services.renater.fr/tcs/faq/tcs_personnes/export_import#importer_une_sauvegarde_de_certificat_dans_mon_navigateur

.. [5] Conversion d'un certificat : https://doc.cc.in2p3.fr/fr/Daily-usage/faq/faq-general-help.html#convertir-un-certificat
