
.. Document meta

:orphan:

.. |antsibull-internal-nbsp| unicode:: 0xA0
    :trim:

.. role:: ansible-attribute-support-label
.. role:: ansible-attribute-support-property
.. role:: ansible-attribute-support-full
.. role:: ansible-attribute-support-partial
.. role:: ansible-attribute-support-none
.. role:: ansible-attribute-support-na
.. role:: ansible-option-type
.. role:: ansible-option-elements
.. role:: ansible-option-required
.. role:: ansible-option-versionadded
.. role:: ansible-option-aliases
.. role:: ansible-option-choices
.. role:: ansible-option-choices-default-mark
.. role:: ansible-option-default-bold
.. role:: ansible-option-configuration
.. role:: ansible-option-returned-bold
.. role:: ansible-option-sample-bold

.. Anchors

.. _ansible_collections.skupper.network.services_load_module:

.. Anchors: short name for ansible.builtin

.. Title

skupper.network.services_load module -- Loads existing services and targets
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. Collection note

.. note::
    This module is part of the `skupper.network collection <https://galaxy.ansible.com/skupper/network>`_ (version 1.1.3).

    To install it, use: :code:`ansible-galaxy collection install skupper.network`.
    You need further requirements to be able to use this module,
    see :ref:`Requirements <ansible_collections.skupper.network.services_load_module_requirements>` for details.

    To use it in a playbook, specify: :code:`skupper.network.services_load`.

.. version_added

.. rst-class:: ansible-version-added

New in skupper.network 1.1.3

.. contents::
   :local:
   :depth: 1

.. Deprecated


Synopsis
--------

.. Description

- Loads existing Skupper services and targets. Existing services will be returned under the \`existing\_services\` fact.

.. note::
    This module has a corresponding :ref:`action plugin <action_plugins>`.

.. Aliases


.. Requirements

.. _ansible_collections.skupper.network.services_load_module_requirements:

Requirements
------------
The below requirements are needed on the host that executes this module.

- kubectl if using kubernetes platform
- podman v4+ if using podman as the site platform






.. Options


.. Attributes


.. Notes


.. Seealso


.. Examples

Examples
--------

.. code-block:: yaml+jinja

    
    - name: Loading existing services
      skupper.network.services_load:




.. Facts


.. Return values

Return Values
-------------
Common return values are documented :ref:`here <common_return_values>`, the following are the fields unique to this module:

.. rst-class:: ansible-option-table

.. list-table::
  :width: 100%
  :widths: auto
  :header-rows: 1

  * - Key
    - Description

  * - .. raw:: html

        <div class="ansible-option-cell">
        <div class="ansibleOptionAnchor" id="return-existing_services"></div>

      .. _ansible_collections.skupper.network.services_load_module__return-existing_services:

      .. rst-class:: ansible-option-title

      **existing_services**

      .. raw:: html

        <a class="ansibleOptionLink" href="#return-existing_services" title="Permalink to this return value"></a>

      .. rst-class:: ansible-option-type-line

      :ansible-option-type:`dictionary`

      .. raw:: html

        </div>

    - .. raw:: html

        <div class="ansible-option-cell">

      List of existing services and targets


      .. rst-class:: ansible-option-line

      :ansible-option-returned-bold:`Returned:` always

      .. rst-class:: ansible-option-line
      .. rst-class:: ansible-option-sample

      :ansible-option-sample-bold:`Sample:` :ansible-rv-sample-value:`{"existing\_services": {"db": {"ports": [5432]}, "nearestprime": {"ports": [8000], "targets": [{"name": "nearestprime", "type": "deployment"}]}}}`


      .. raw:: html

        </div>



..  Status (Presently only deprecated)


.. Authors



.. Extra links

Collection links
~~~~~~~~~~~~~~~~

.. raw:: html

  <p class="ansible-links">
    <a href="http://github.com/skupperproject/skupper-ansible/issues" aria-role="button" target="_blank" rel="noopener external">Issue Tracker</a>
    <a href="http://skupper.io" aria-role="button" target="_blank" rel="noopener external">Homepage</a>
    <a href="http://github.com/skupperproject/skupper-ansible" aria-role="button" target="_blank" rel="noopener external">Repository (Sources)</a>
  </p>

.. Parsing errors

