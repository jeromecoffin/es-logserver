# es-logserver

log server with Docker, Elasticsearch, Kibana and Nginx


![diagram](/diagramlogstash.png)


[Kibana](https://www.elastic.co/products/kibana)
- Internal Port : 5601
- Image : docker.elastic.co/kibana/kibana:6.1.2

[ElasticSearch](https://www.elastic.co/products/elasticsearch)
- Internal Port : 9200
- Image : elastic.co/elasticsearch/elasticsearch:6.3.2

[Nginx](https://www.nginx.com/)
- Internal port : 80
- External port : 8080
- Image : nginx
- Configuration : nginx.conf and .htpasswd

[Logstash](https://www.elastic.co/products/logstash)
- Port : 5000/tcp
- Port : 5000/udp
- Port : 9600
- miage : docker.elastic.co/logstash/logstash:6.8.6


## Quick Start Guide

Import log file
```
$ cat /path/to/file/file.log | nc -c localhost 5000 
```

Launch the log server
```
$ docker-compose build
$ docker-compose up -d
$ docker-compose ps -a
```

## Soon

[Filebeat](https://www.elastic.co/products/beats/filebeat)
