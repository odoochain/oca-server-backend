=========================
External Database Sources
=========================

..
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! source digest: sha256:b6b6d53c12bad99b5a75536b07a9b3de684f59baadf1b10f4612f5f25640b26d
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-LGPL--3-blue.png
    :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
    :alt: License: LGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fserver--backend-lightgray.png?logo=github
    :target: https://github.com/OCA/server-backend/tree/16.0/base_external_dbsource
    :alt: OCA/server-backend
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/server-backend-16-0/server-backend-16-0-base_external_dbsource
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
    :target: https://runboat.odoo-community.org/builds?repo=OCA/server-backend&target_branch=16.0
    :alt: Try me on Runboat

|badge1| |badge2| |badge3| |badge4| |badge5|

This module allows you to define connections to foreign databases using ODBC,
Firebird, Oracle Client or SQLAlchemy.

**Table of contents**

.. contents::
   :local:

Installation
============

No installation required.

Configuration
=============

To configure this module, you need to:

#. Database sources can be configured in Settings > Technical >
   Database Structure > Data sources.

Usage
=====

* Go to Settings > Technical > Database Structure > Database Sources
* Click on Create to enter the following information:

* Data source name
* Password
* Connector: Choose the database to which you want to connect
* Connection string: Specify how to connect to database

Known issues / Roadmap
======================

* Find a way to remove or default the CA certs dir
* Add concept of multiple connection strings for one source (multiple nodes)
* Add a ConnectionEnvironment that allows for the reuse of connections
* Message box should be displayed instead of error in ``connection_test``
* Remove old api compatibility layers (v11)
* Instead of returning list of results, we should return iterators. This will
  support larger datasets in a more efficient manner.
* Implement better CRUD handling

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/server-backend/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us to smash it by providing a detailed and welcomed
`feedback <https://github.com/OCA/server-backend/issues/new?body=module:%20base_external_dbsource%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* Daniel Reis
* LasLabs

Contributors
~~~~~~~~~~~~

* Daniel Reis <dreis.pt@hotmail.com>
* Maxime Chambreuil <maxime.chambreuil@savoirfairelinux.com>
* Gervais Naoussi <gervaisnaoussi@gmail.com>
* Dave Lasley <dave@laslabs.com>

* `Tecnativa <https://www.tecnativa.com>`_:

  * Sergio Teruel
  * Jairo Llopis
  * Andrea Cattalani (`Moduon <https://www.moduon.team/>`__)

Maintainers
~~~~~~~~~~~

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

This module is part of the `OCA/server-backend <https://github.com/OCA/server-backend/tree/16.0/base_external_dbsource>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
