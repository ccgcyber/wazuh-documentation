.. Copyright (C) 2018 Wazuh, Inc.

.. _wazuh_docker:

Docker
======

`Docker <https://www.docker.com/>`_ is an open-source project that automates the deployment of different applications inside software containers. Docker containers wrap up a piece of software in a complete filesystem that contains everything it needs to run like: code, system tools, libraries, etc. This process guarantees that the system will always run the same, regardless the environment it is running.

We have created our own fork based on `"deviantony" dockerfiles <https://github.com/deviantony/docker-elk>`_ and `"xetus-oss" dockerfiles <https://github.com/xetus-oss/docker-ossec-server>`_. Thank you, Anthony Lapenna, for your contribution to the community. If you want to contribute to the Wazuh fork, please go to the `Wazuh docker repository <https://github.com/wazuh/wazuh-docker>`_

The images we created are in the `Docker hub <https://hub.docker.com>`_. You can install Wazuh with a single-host architecture using a set of Docker images that contains `Wazuh Manager <https://github.com/wazuh/wazuh>`_, `Wazuh API <https://github.com/wazuh/wazuh-api>`_, `Filebeat <https://www.elastic.co/products/beats/filebeat>`_, `Logstash <https://registry.hub.docker.com/_/logstash/>`_, `Elasticsearch <https://registry.hub.docker.com/_/elasticsearch/>`_, `Kibana <https://registry.hub.docker.com/_/kibana/>`_

This section will show you the process:

.. toctree::
   :maxdepth: 2

   docker-installation
   wazuh-container
   faq-wazuh-container
