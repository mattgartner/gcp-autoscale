## Send traffic to the load balancer
Send 5,000 requests from a single client - ~64 RPS
```
ab -n 5000 -c 1 http://phx.mattgartner.org/
```
Send 15,000 requests via 100 clients - ~6350 RPS
```
ab -n 15000 -c 100 http://phx.mattgartner.org/
```

## Build the Docker Image
```
docker build -t nginx .
```

[optional to test locally]
```
docker run --rm -it -p 8080:80 nginx
```
```
docker tag nginx gcr.io/onboard-phx-scaling/nginx
```
```
docker push gcr.io/onboard-phx-scaling/nginx
```