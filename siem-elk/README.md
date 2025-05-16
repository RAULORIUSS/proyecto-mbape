
## Iniciar servicios

```
$ docker compose up -d
```
## Parar servicios
```
$ docker compose down
```
## Servicios

* Elasticsearch: [`http://localhost:9200`](http://localhost:9200)
* Logstash: [`http://localhost:9600`](http://localhost:9600)
* Kibana: [`http://localhost:5601`](http://localhost:5601)


## ataques 

### intento fallido de ssh
ssh usuario@localhost -p 2222

### escaneo de puertos
nmap -sV -Pn -p 2222 localhost

### ataque ddos simulado 

nmap -p 2222 --script ssh-brute --script-args userdb=users.txt,passdb=passwords.txt,brute.threads=100,ssh.user=root 127.0.0.1