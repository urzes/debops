.. Copyright (C) 2021 Julien Lecomte <julien@lecomte.at>
.. Copyright (C) 2021 DebOps <https://debops.org/>
.. SPDX-License-Identifier: GPL-3.0-only

Getting started
===============

Default configuration
---------------------

The service will be configured to serve run a Zabbix monitoring agent.

Example inventory
-----------------

To enable the Zabbix agent service on a host it needs to be included in the specific Ansible
inventory group:

.. code-block:: none

   [debops_service_zabbix_agent]
   hostname


Example playbook
----------------

If you are using this role without DebOps, here's an example Ansible playbook
that uses the ``debops.zabbix_agent`` role:

.. literalinclude:: ../../../../ansible/playbooks/service/zabbix_agent.yml
   :language: yaml
   :lines: 1,5-
