Certificate Request for CNRS Employees
======================================

Introduction
------------

This documentation outlines the procedure to obtain a TCS [1]_
certifcate for CNRS employees. These certificates are issued to
facilitate access to grid computing resources, cloud services, and
secure websites.

This guide is based on the CNRS reference documentation [2]_.

**Note:** The user is responsible for ensuring the custody and
backup of the private keys of the issued certificates.


Obtaining a Certificate
-----------------------

It is only possible to obtain a CNRS certificate for agents with
a JANUS identifier pointing to an e-mail address in a domain
managed by the CNRS. If this is not the case, you must go
through the authority that owns the domain name. For example, for
the staff of the Creatis laboratory, whose domain name is managed by
INSA, you need to contact the INSA to obtain a certificate.

To obtain a certificate, follow these steps:

1. Connect to the SESAME portal: https://sesame.cnrs.fr/

2. Click on "Manage my certificates".

3. Identify yourself using your CNRS identifiers. To do this
   select "CNRS - Unit staff" and go to the next step.
   You will then be asked to identify yourself with your
   Janus identifiers.

4. Order a certificate by clicking on the "Request a new personal
   certificate" button

5. Choose a strong password to protect the certificate [3]_.

6. The generated certificate is then automatically downloaded to
   your computer.


In case of problems
-------------------

If you have any issues generating your certificate, you can contact
the SESAME support team by clicking on the "Support" link in the
bottom right-hand corner.

Conversion and import
--------------------

The downloaded certificate is in PKCS12 format. It can be loaded into
the browser [4]_ or transformed into x509 format for use with the
computing grid tools [5]_.


.. [1] TCS Certificate: https://wiki.geant.org/display/TCSNT/TCS+wiki+%282020%29+Sectigo

.. [2] Official SESAME Documentationi (fr): https://aide.core-cloud.net/certificats/Pages/PersonnelDemanderCertificat.aspx

.. [3] ANSSI Recommandations concerning the password creation (fr): https://cyber.gouv.fr/cybermois-2021-les-mots-de-passe

.. [4] Loading a certificate in a browser (fr): https://services.renater.fr/tcs/faq/tcs_personnes/export_import#importer_une_sauvegarde_de_certificat_dans_mon_navigateur 
i
.. [5] Converting a certificate: https://doc.cc.in2p3.fr/en/Daily-usage/certificate.html#certificate
