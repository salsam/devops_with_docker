# Example frontend and backend deployment

Example backend and frontend were deployed to AWS EC2 with `docker-compose.yml` that can be seen in this directory. For app see manager node's address `http://ec2-34-245-208-57.eu-west-1.compute.amazonaws.com`. Swarm also has two worker nodes `ec2-34-245-235-86.eu-west-1.compute.amazonaws.com` and `ec2-34-241-6-95.eu-west-1.compute.amazonaws.com`.

## Deployment

```bash
[ec2-user@ip-172-31-21-215 ~]$ docker service ls
ID                  NAME                     MODE                REPLICAS            IMAGE                                    PORTS
rrhgg16n0teu        swarm-example_backend    replicated          1/1                 cyansea/backend-example-docker:latest    *:8000->8000/tcp
kw749qj62u4s        swarm-example_frontend   replicated          1/1                 cyansea/frontend-example-docker:latest   *:5000->5000/tcp
iq91lh9nnvof        swarm-example_postgres   replicated          1/1                 postgres:latest                          *:5432->5432/tcp
mb31d5ixcqku        swarm-example_proxy      replicated          1/1                 jwilder/nginx-proxy:latest               *:80->80/tcp
20tigd6y70z9        swarm-example_redis      replicated          1/1                 redis:latest                             *:6379->6379/tcp
```