# Ansible Elasticsearch Role

## What it does
Installs java, Elasticsearch and installs configs with passed in params.

Sets an iptables rule which allows ingress connections from other cluster hosts

## Usage
Install in roles and call from playbook with:

```
- hosts: elasticsearch_servers
   - {
     role: elasticsearch,
     cluster_name: clust,
     zone: zone1,
     iplist: ['10.10.0.10', '10.10.0.11']
    }

```

## Notes
