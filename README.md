Ansible ElasticSearch-Kibana Role
=========

- Install&Configure single node or cluster ElasticSearch5 with Kibana extension. 
- Configure Linux kernel parameter for ElasticSearch5


Requirements
------------
This role requires,

- Ansible 1.4 or higher and platform requirements.
- This role support Elasticsearch 5 version.
- This role support Ubuntu 14.04 or higher operating system.

Role Variables
--------------
You can find role variables below. You must change ES_CLUSTER value to false for a single node.

```
ES_VERSION: 5.1.2
KIBANA_VERSION: 5.1.2
HEAP_SIZE: 4g
CLUSTER_NAME: ELASTIC_CLUSTER
ES_CLUSTER: "true"
NODE1_IP: 192.168.40.50
NODE2_IP: 192.168.40.51
NODE3_IP: 192.168.40.52
KIBANA_SERVER_HOST: 0.0.0.0
```


Example Playbook
----------------
```
---
- name: Install ElasticSearch Cluster
  hosts: all
  roles:
    - elasticsearch-kibana
```
