# es-logserver
log server with Docker, Elasticsearch, Kibana and Nginx

![diagram](/diagram.png)

[Kibana](https://www.elastic.co/products/kibana)
- Internal Port : 5601
- Base Image : docker.elastic.co/kibana/kibana:6.1.2

[ElasticSearch](https://www.elastic.co/products/elasticsearch)
- Internal Port : 9200
- Image : elastic.co/elasticsearch/elasticsearch:6.3.2

[Nginx](https://www.nginx.com/)
- Internal port : 80
- External port : 8080
- Image : nginx
- Configuration : nginx.conf and .htpasswd



## Quick Start Guide

1) to start with
```
$ docker-compose up -d
```

## Soon

[Filebeat](https://www.elastic.co/products/beats/filebeat)

[Logstash](https://www.elastic.co/products/logstash)
