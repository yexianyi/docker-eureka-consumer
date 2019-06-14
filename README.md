### Usage:
```
docker network create eureka-net
docker run -it --rm --net eureka-net -e EUREKA_CONSUMER_PORT=8900 -e EUREKA_SERVER_PEER_URL=http://172.24.155.70:8761/eureka -p8900:8900 -d yexianyi/eureka-consumer
```
### Note:
1) EUREKA_CONSUMER_PORT: Consumer Service Port
2) EUREKA_SERVER_PEER_URL: Eureka Registry Url

### Example:
```
curl -X GET -i 'http://localhost:8900/ribbon-consumer?message=abc'
```
