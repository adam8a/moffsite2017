# moffsite2017
2017 offsite project


Mlaunch-like tool to create yaml definition files for docker containers
Spin up the N docker containers from these yaml files: M as servers, K as clients
Run loads on the K clients (POCDriver?) to stress the cluster
Auto collect diagnostic.data and load into mseries to to analyze

Yaml files:
Examples for yaml files for a sharded cluster:  
[mongodb-swarm demo](https://github.com/sisteming/mongodb-swarm/tree/master/demo)  
[mdb_cgroup.yaml](https://github.com/sisteming/mongodb-swarm/blob/master/demo/mdb_cgroup.yaml)


Start w/3 sets of yaml files:
Small: PSS with 1 client
Medium: 2 PSS Shards, 3 configs (csrs), 2 mongos, 2 clients
Large: 8 PSS Shards, 5 configs (csrs), 4 mongos, 4 clients

===

PocDriver: https://github.com/johnlpage/POCDriver
