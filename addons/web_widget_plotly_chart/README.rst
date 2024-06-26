=================
Web Widget Plotly
=================

.. 
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! source digest: sha256:e5f2ea60f70bb2f141322599481e405f38bff060dd65cdcdb6f06b366e83e7a2
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-LGPL--3-blue.png
    :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
    :alt: License: LGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fweb-lightgray.png?logo=github
    :target: https://github.com/OCA/web/tree/17.0/web_widget_plotly_chart
    :alt: OCA/web
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/web-17-0/web-17-0-web_widget_plotly_chart
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
    :target: https://runboat.odoo-community.org/builds?repo=OCA/web&target_branch=17.0
    :alt: Try me on Runboat

|badge1| |badge2| |badge3| |badge4| |badge5|

This module add the possibility to insert Plotly charts into Odoo
standard views.

.. image:: https://raw.githubusercontent.com/OCA/web/17.0/web_widget_plotly_chart/static/description/example.png
   :alt: Plotly Chart inserted into an Odoo view

`Plotly <https://plot.ly/>`__ is a Python interactive visualization
library built on top of d3.js and stack.gl, plotly.js is a high-level,
declarative charting library. plotly.js ships with over 40 chart types,
including scientific charts, 3D graphs, statistical charts, SVG maps,
financial charts, and more.

If you want to see some samples of plotly's capabilities follow this
`link <https://github.com/plotly/plotly.py#overview>`__.

**Table of contents**

.. contents::
   :local:

Installation
============

You need to install the python plotly library:

::

   pip install plotly==5.22.0

Usage
=====

To insert a Plotly chart in a view proceed as follows:

1. Import plotly:

   import plotly

2. Declare a text computed field like this:

   ::

      plotly_chart = fields.Text(
          string='Plotly Chart',
          compute='_compute_plotly_chart',
      )

3. In its computed method do:

   ::

      def _compute_plotly_chart(self):
          for rec in self:
              data = [{'x': [1, 2, 3], 'y': [2, 3, 4]}]
              rec.plotly_chart = plotly.offline.plot(data,
                                           include_plotlyjs=False,
                                           output_type='div')

4. In the view, add something like this wherever you want to display
   your plotly chart:

   ::

      <div>
          <field name="plotly_chart" widget="plotly_chart" nolabel="1"/>
      </div>

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/web/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us to smash it by providing a detailed and welcomed
`feedback <https://github.com/OCA/web/issues/new?body=module:%20web_widget_plotly_chart%0Aversion:%2017.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
-------

* LevelPrime srl

Contributors
------------

-  Roberto Fichera <roberto.fichera@levelprime.com>
-  Michele Zaccheddu <michele.zaccheddu@levelprime.com>

Other credits
-------------

-  This module uses the library
   `Plotly.js <https://github.com/plotly/plotly.js>`__ which is under
   the open-source MIT License. Copyright (c) 2019 Plotly, Inc
-  Odoo Community Association (OCA)

Maintainers
-----------

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

.. |maintainer-robyf70| image:: https://github.com/robyf70.png?size=40px
    :target: https://github.com/robyf70
    :alt: robyf70

Current `maintainer <https://odoo-community.org/page/maintainer-role>`__:

|maintainer-robyf70| 

This module is part of the `OCA/web <https://github.com/OCA/web/tree/17.0/web_widget_plotly_chart>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
