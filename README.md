# Ender's Cassandra

Apache Cassandra Ansible Role

Setup local testing environment quickly and easily.

# Features

- \[DOING\] Cassandra Cluster
- \[TODO\] Reaper
- \[TODO\] Medusa
- \[TODO\] JMX Exporter

# Variables

- `cassandra_version`, Cassandra version, default is `4.0.7`
- `cassandra_home`, Cassandra home directory, default is `/opt/cassandra`
- `assandra_ip_address` **RECOMMENDED**, node external ip address
- `cassandra_cluster_name`, Cassandra cluster name, default is `Test Cluster`
- `cassandra_data_directory`, Cassandra data directory, default is `/data/cassandra/data`
- `cassandra_commitlog_directory`, Cassandra commit log directory, default is `/data/cassandra/commitlog`
- `cassandra_hints_directory`, Cassandra hints directory, default is `/data/cassandra/hints`
- `cassandra_saved_caches_directory`, Cassandra saved caches directory, default is `/data/cassandra/saved_caches`

# Demo

Setup the VMs:

```
vagrant up
```

Deploy:

```
ansible-playbook deploy.yml
```
