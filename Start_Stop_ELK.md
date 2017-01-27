# How to start and Stop ELK ?

## Elastic Search

Below parameter determines the elastic search host url. If you planning to use localhost you can just comment this part.   

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

### How to check ElasticSearch is running ?

Launch the below url in the browser.  

```
http://localhost:9200/
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
