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

Elastic Search configuration is available in below path.  

```
<Elastic Seartch Download >/config/elasticsearch.yml 
```

[Start and Stop Elastic Search](https://github.com/dilipthelip/LearnELK/blob/master/Start_Stop_ELK.md)
### ElasticSearch Cluster:

- ElasticSearch cluster is a bunch of nodes , each node is a running instance of elastic search.
- Each node stores data, participates in cluster searching and indexing capabilities. Each node will be assigned a random marvel character name.
- When you start a node it tries to find and join a cluster defined in elasticsearch.yml file.

### Nodes:
Go through the below link.  

https://www.elastic.co/guide/en/elasticsearch/reference/current/modules-node.html

### Index in ElasticSearch:  
- An index is a collection of document with similar characteristics.
- Index is identified by a name and it must be in lowercase.
- Used in searching, indexing, updating and deleting documents within index.
- You can define as many as indexes you want in a cluster.
- Inside each index there can be multiple **TYPES**. Each type corresponds to one particular type.  
  For Eg., :- company index type and employee index type.  
- Each JSON object is considered as a document and these are store in an index. Each document has a bunch of **fields** in it.

**FIELDS:**  
- Each field has a type. It could be Text, Date, Number and so on.  

### ElasticSearch Analogy to RDBMS:
RDBMS       |   ElasticSearch  
Database    |   Index  
Table       |   Type  
Column      |   Field  
Row         |   Document  

### Shards:  
- All the data in the index is stored as SHRADS.  
- Index is divided in to multiple pieces called shrads.  
- We need to define shrads when creating an Index.  

### Replica:  
- Replica is a copy of a shrad, each shrad can have one or more replicas.
- A primary shrad is the place where the document is stored.
- Primary shrad and replica shrad must be in different nodes.  
- By default 5 primary shrads and 1 replica shrad for each index in elastic search.  




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







