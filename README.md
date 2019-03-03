# gcp-autoscale

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