# moffsite2017
2017 offsite project

RaaS: Reproduction as a Service

- Mlaunch-like tool to create yaml definition files for docker containers
- Spin up the N docker containers from these yaml files: M as servers, K as clients
- Run loads on the K clients (POCDriver?) to stress the cluster
- Auto ciollect diagnostic.data and load into mseries to to analyze

Yaml files:
Examples for yaml files for a sharded cluster:
https://github.com/sisteming/mongodb-swarm/tree/master/demo

Start w/3 sets of yaml files:
- Small: PSS with 1 client
- Medium: 2 PSS Shards, 3 configs (csrs), 2 mongos, 2 clients
- Large: 8 PSS Shards, 5 configs (csrs), 4 mongos, 4 clients
===

PocDriver: https://github.com/johnlpage/POCDriver

Dave’s alternative idea:
Extend https://github.com/10gen/dsi/ so that it’s easy to setup clusters yourself (not in Evergreen).
Make DSI infrastructure integrate with Docker.
