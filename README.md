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


## Ingress:

Added ingress via ingress-nginx. (see https://kubernetes.github.io/ingress-nginx/deploy/)

Updated host file (/etc/hosts) to include posts.com as redirect when attempting to connect to localhost (127.0.0.1 posts.com) 