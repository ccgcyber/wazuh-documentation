.. Copyright (C) 2018 Wazuh, Inc.

.. _setup_puppet_agent:

Installing Puppet agent
============================

In this section we assume you have already installed the ``apt`` or ``yum`` Puppet repository on your agent system in the same way that you did on your Puppet Server.

Installation on CentOS/RHEL/Fedora
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: console

   # yum install puppet
   # puppet resource package puppet ensure=latest

Installation on Debian/Ubuntu
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: console

   # apt-get install puppet
   # apt-get update
   # puppet resource package puppet ensure=latest

Configuration
^^^^^^^^^^^^^

Add the server value to the ``[main]`` section of the node’s ``/etc/puppet/puppet.conf`` file, replacing ``puppet.example.com`` with your Puppet Server’s FQDN::

   [main]
   server = puppet.example.com

Restart the Puppet service:

.. code-block:: console

   # service puppet restart
