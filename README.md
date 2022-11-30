# Elastic Search Demo

## Usage
```bash
cp .env.sample .env
vi .env // Please set info by your env

docker compose build
docker compose up
```

## Test
```bash
curl localhost:9200
```

When you got like the below response, the Elastic search is working well.

```json
{
  "name" : "xxxxxxxxxxxx",
  "cluster_name" : "docker-cluster",
  "cluster_uuid" : "xxxxxxxxxxxxxxx",
  "version" : {
    "number" : "8.5.2",
    "build_flavor" : "default",
    "build_type" : "docker",
    "build_hash" : "xxxxxxxxxxxxxxxxxxxx",
    "build_date" : "2022-11-17T18:56:17.538630285Z",
    "build_snapshot" : false,
    "lucene_version" : "9.4.1",
    "minimum_wire_compatibility_version" : "7.17.0",
    "minimum_index_compatibility_version" : "7.0.0"
  },
  "tagline" : "You Know, for Search"
}
```
