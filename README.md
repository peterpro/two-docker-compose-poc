# two-docker-compose-poc

``` 
docker network create hwexternal
docker-compose -p hello1_project -f docker-compose.hw1.yml up -d
docker-compose -p hello2_project -f docker-compose.hw2.yml up -d
 
docker exec -it hello1_project_hw_1 ping hello2_project_hw_1
```
 
#64 bytes from 192.168.160.3: seq=0 ttl=64 time=0.232 ms 

#64 bytes from 192.168.160.3: seq=1 ttl=64 time=0.169 ms
