# es-logserver
log server with Docker, Elasticsearch, Kibana and Nginx

![diagram](/diagram.png)

Kibana
- Internal Port : 5601
- Base Image : docker.elastic.co/kibana/kibana:6.1.2

Elastic Search
- Internal Port : 9200
- Image : elastic.co/elasticsearch/elasticsearch:6.3.2

Nginx
- Internal port : 80
- External port : 8080
- Image : nginx
- Configuration : nginx.conf and .htpasswd
