# Docker Compose Elasticsearch and Kibana

# How to run
* Create docker network
```
docker network create elastic
```
* Run docker compose
```
docker compose up
```
* Check docker container was started
```
─➤  curl localhost:9200
{
  "name" : "964d7c24ec0e",
  "cluster_name" : "docker-cluster",
  "cluster_uuid" : "V0y4YkaWT_KVRRuSrMPStw",
  "version" : {
    "number" : "8.2.2",
    "build_flavor" : "default",
    "build_type" : "docker",
    "build_hash" : "9876968ef3c745186b94fdabd4483e01499224ef",
    "build_date" : "2022-05-25T15:47:06.259735307Z",
    "build_snapshot" : false,
    "lucene_version" : "9.1.0",
    "minimum_wire_compatibility_version" : "7.17.0",
    "minimum_index_compatibility_version" : "7.0.0"
  },
  "tagline" : "You Know, for Search"
}

```