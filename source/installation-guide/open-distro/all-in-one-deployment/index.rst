.. Copyright (C) 2020 Wazuh, Inc.

.. _all_in_one_index:

All-in-one deployment
=====================

This section guides through the installation and configuration of the Wazuh server and Elastic Stack on the same host. This type of deployment is appropriate for testing and small production environments.

The following components will be installed:

- The Wazuh server, including the Wazuh manager as a single-node cluster and the Wazuh API.

- Elastic Stack, including Open Distro for Elasticsearch as a single-node cluster, Filebeat, and Open Distro for Kibana including the Wazuh Kibana plugin.

The communication will be encrypted using SSL certificates. Those certificates will be generated using the `Search Guard offline TLS tool <https://docs.search-guard.com/latest/offline-tls-tool>`_. The guide will also refer to the section explaining how to secure communication between the Wazuh API and the Wazuh Kibana plugin.
Besides, in order to use the Wazuh Kibana plugin properly, the extra Elasticsearch roles and users will be added.

To allow the installation process and guarantee the expected performance of the Wazuh components the host must meet the hardware requirements described in the :ref:`requirements <all_in_one_requirements>` section.

The user can choose between Step-by-step installation, a manual way of carrying out the process, and Unattended installation, an automated way using a script:

.. toctree::
    :maxdepth: 1
    :hidden:

    requirements

.. toctree::
    :maxdepth: 1
    :glob:

    unattended-installation
    all_in_one