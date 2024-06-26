============================
Field Service - Flow for ISP
============================

.. 
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! source digest: sha256:d82a5e99e72df7399e0a0d7e4e2cc9a8abf04eb183d44edc9a7af4e46b4342a8
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Ffield--service-lightgray.png?logo=github
    :target: https://github.com/OCA/field-service/tree/17.0/fieldservice_isp_flow
    :alt: OCA/field-service
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/field-service-17-0/field-service-17-0-fieldservice_isp_flow
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
    :target: https://runboat.odoo-community.org/builds?repo=OCA/field-service&target_branch=17.0
    :alt: Try me on Runboat

|badge1| |badge2| |badge3| |badge4| |badge5|

This module is an add-on for the Field Service application in Odoo. It
provides default stages for orders and some validation logic when
changing current stage.

**Table of contents**

.. contents::
   :local:

Configuration
=============

The stage of an order is used to monitor its progress. Stages can be
configured based on your company's specific business needs. A basic set
of order stages comes pre-configured for use.

1. Go to *Field Service > Configuration > Stages*
2. Create or edit a stage
3. Set the name for the stage.
4. Set the sequence order for the stage.
5. Select *Order* type to apply this stage to your orders.
6. Additonally, you can set a color for the stage.

Usage
=====

To use this module, you need to:

-  Create a new service order
-  Under the Inventory tab, select the warehouse, the delivery method
   and add products with quantity
-  Confirm the order to create the delivery orders with the selected
   method

Known issues / Roadmap
======================

The roadmap of the Field Service application is documented on
`Github <https://github.com/OCA/field-service/issues/1>`__.

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/field-service/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us to smash it by providing a detailed and welcomed
`feedback <https://github.com/OCA/field-service/issues/new?body=module:%20fieldservice_isp_flow%0Aversion:%2017.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
-------

* Open Source Integrators
* Akretion

Contributors
------------

-  Maxime Chambreuil <mchambreuil@opensourceintegrators.com>
-  Serpent Consulting Services Pvt. Ltd. <support@serpentcs.com>
-  Raphaël Reverdy <raphael.reverdy@akretion.com>
-  Freni Patel <fpatel@opensourceintegrators.com>
-  [APSL](https://apsl.tech):

   -  Antoni Marroig <amarroig@apsl.net>

Other credits
-------------

The development of this module has been financially supported by:

-  Open Source Integrators <https://opensourceintegrators.com>

Maintainers
-----------

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

.. |maintainer-osi-scampbell| image:: https://github.com/osi-scampbell.png?size=40px
    :target: https://github.com/osi-scampbell
    :alt: osi-scampbell

Current `maintainer <https://odoo-community.org/page/maintainer-role>`__:

|maintainer-osi-scampbell| 

This module is part of the `OCA/field-service <https://github.com/OCA/field-service/tree/17.0/fieldservice_isp_flow>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
