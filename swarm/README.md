# Demo with Swarm

```
docker swarm init
docker node ls
docker stack deploy --compose-file docker-compose.yml demo

docker service ls
ID             NAME       MODE         REPLICAS   IMAGE     PORTS
oc8vzlnupcec   demo_web   replicated   1/1        web:4.0   *:9999->80/tcp
```

Scaling
```
docker service scale demo_web=5
```

Leave 
```
docker swarm leave -f
```