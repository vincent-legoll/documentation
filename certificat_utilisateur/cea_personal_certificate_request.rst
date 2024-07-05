Certificate Request for CEA/DRF/IRFU Employees
==============================================

Introduction
------------

This documentation outlines the procedure to obtain a TCS [1]_
certificate for CEA/DRS/IRFU employees. These certificates are issued
to facilitate access to grid computing resources (like WLCG [2]_),
cloud services, and secure websites.

**Note:** The user is responsible for ensuring the custody and
backup of the private keys of the issued certificates.


Obtaining a Certificate
-----------------------

To obtain a certificate, follow these steps:

1. Connect to the TCS Certificate portal: https://cert-manager.com/customer/renater/idp/clientgeant

2. Identify yourself with the CEA identity federation, by choosing:
   CEA French Alternatives Energies ans Atomic Energy Commission and
   authenticate with your identifiers (AB123456 + mobipass)

3. Select the Certificate Profile: "GEANT Personal Authentication" and
   fill in the fields :

   * Enrollment Method: KeyGEneration

   * Key Type: RSA - 2048

   * Strong password [3]_

   * Algorithm: AES256-SHA256

4. The generated certificate is then automatically generated and
   downloaded to your computer as the ``certs.p12`` file.


Conversion and import
---------------------

The downloaded certificate is in PKCS12 format. It can be loaded into
the browser [4]_ or transformed into x509 format for use with the
computing grid tools [5]_.


.. [1] TCS Certificate: https://wiki.geant.org/display/TCSNT/TCS+wiki+%282020%29+Sectigo

.. [2] Official SESAME Documentationi (fr): https://aide.core-cloud.net/certificats/Pages/PersonnelDemanderCertificat.aspx

.. [3] ANSSI Recommandations concerning the password creation (fr): https://cyber.gouv.fr/cybermois-2021-les-mots-de-passe

.. [4] Loading a certificate in a browser (fr): https://services.renater.fr/tcs/faq/tcs_personnes/export_import#importer_une_sauvegarde_de_certificat_dans_mon_navigateur

.. [5] Converting a certificate: https://doc.cc.in2p3.fr/en/Daily-usage/certificate.html#certificate
