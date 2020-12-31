# blog
microservices


## Docker:

build:
docker build -t [hub username]/[image name]:[version defaults latest]

push build to hub:
docker push [hub username]/[image name]:[version defaults latest]


## Kubernetes:

apply:
kubectl apply -f [hub image name]:[Version defaults latest]

See logs:
kubectl logs [pod name]

After deployment is updated:
kubectl rollout restart deployment [deployment name]