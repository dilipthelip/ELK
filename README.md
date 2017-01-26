# ELK

## Elastic Search:  
- Elastic search is a NOSQL database. 
- This is developed based on Apache Lucence.
- Developed based on Java.
- Distributed document store and uses JSON over a RESTFUL Api.
- Schema-less
- Its highly available because these always run on a cluster which has multiple nodes.
- It uses resful api to access the elastic search indexes.
- **MultiTenancy-** Different nodes are used by different clients.
- Enable alerts and notifications using **Percolating**.  

### How to download elasticsearch ?

Download elastic search from the below link.  

[Download Elastic Search](https://www.elastic.co/downloads/elasticsearch)

Elastic Searcg configuration is available in below path.  

```
<Elastic Seartch Download >/config/elasticsearch.yml 
```

Below parameter determines the host url.If you planning to use localhost you can just comment this part.   

```
#network.host: 192.168.0.1
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
- Process logs and sends it to different types of output sources.
- It can convert different data sources in to one single format.
- Fields extraction in logstash for elastic search.
- 

## Kibana
- This is a visualization tool.
- Provides the web-gui to visualize any kind of data stored in ElasticSearch indexes.
- Uses the search and indexing capabilities of Elastic Search through Restful API to display graphics through end users.
- Provides histograms, pie charts, column charts, tables, maps etc.,

Configuration is available in below path.  

```
<Kibana Download Version>/config/kibana.yml

```

#### How Kibana connects to elastic search ?

The **Kibana.yml** file has the below property which links the Kibana with elastic search.  

```
#elasticsearch.url: "http://localhost:9200"
```

### How to start Kibana ?

```
./kibana

```

As soon as the above command is run Kibana starts listening to the address http://localhost:9200/ .  

By default Kibana runs on port 5601.  

**Kibana URL :** localhost:5601  

### How to install sense plugin in Kibana ?

- Sense plugin helps to search elastic search indexes without using curl command.  
- Sense provides the control of interacting with the elasticsearch.
 
 Navigate to bin directory of Kibana distribution and run the below command.  
 
 Sense is available as part of the distribution itself in Kibana 5.0 and it is available with the name Sense.  
 
 ```
 ./kibana plugin --install elastic/sense
 
 ```







