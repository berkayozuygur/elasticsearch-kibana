ElasticSearch-Kibana
=========

Install&configure standalone or cluster ElasticSearch5 with Kibana extension. 
Configure Linux kernel parameter for ElasticSearch5


Requirements
------------

This role requires Ansible 1.4 or higher and platform requirements.

Role Variables
--------------

You can change standalone or cluster, jvm heap size and elastic&kibana version from defaults site.

Example Playbook
----------------

---
- name: Install ElasticSearch Cluster
  hosts: all
  roles:
    - elasticsearch-kibana

