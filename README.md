# dash-docker-basic

## commands needed for deployment :

docker login -u <user> -p <pass>

### local build
docker build -t dash-prod-example:1.0 -f Dockerfile.prod .

### local run
docker run -d -p 80:80 dash-prod-example:1.0  

### push image to registry
docker image tag dash-prod-example:1.0 pepsomest.azurecr.io/dash-eg:1.0

docker push pepsomest.azurecr.io/dash-eg:1.0 


