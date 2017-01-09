# ELK

## Elastic Search:  
- Elastic search is a NOSQL database
- This is developed based on Apache Lucence.
- Developed based on Java.
- Distributed document store and uses JSON over a RESTFUL Api.
- Schema-less

Configuration is available in below path.  

```
<Elastic Seartch Download >/config/kibana.yml
 
```

### How to start ElasticSearch ?

Approach 1:  
```
./elasticsearch

```

Approach 2:  

```
./elasticsearch --cluster.name XYZ --node.name NODE1

```

### How to run elasticsearch in the background ?

```
./elasticsearch -d

```

### How to stop ElasticSearch running in the background ?

```
ps -ef | grep 'elasticsearch'

kill -9 33467
```

## LogStash:
- Developed using JRuby.

## Kibana
- This is a visualization tool.
- Provides the web-gui to visualize any kind of data stored in ElasticSearch indexes.
- Uses the search and indexing capabilities of Elastic Search through Restful API to display graphics through end users.
- Provides histograms, pie charts, column charts, tables, maps etc.,

Configuration is available in below path.  

```
<Kibana Download Version>/config/kibana.yml

```
