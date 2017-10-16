# docker-elk


Start the ELK stack using `docker-compose`:
```bash
$ docker-compose up --build
```

Stop and remove containers, networks, images, and volumes
```bash
$ docker-compose down
```

Stop services
```bash
$ docker-compose  stop
```

Starts existing containers for a service.
```bash
$ docker-compose  start
```

By default, the stack exposes the following ports:
* 5000: Logstash TCP input.
* 9200: Elasticsearch HTTP
* 9300: Elasticsearch TCP transport
* 5601: Kibana


The shipped Logstash configuration allows you to send content via TCP:
```bash
$ nc localhost 5000 < /path/to/logfile.log
```
