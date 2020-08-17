# docker stack vs kubernetes
These two YAML specification files can deploy what looks like the same stack to your local machine. The sample application is using the dockersamples/k8s-wordsmith-db, dockersamples/k8s-wordsmith-web and dockersamples/k8s-wordsmith-api containers.

## How to deploy
* kubectl apply -f kubernetes.yaml
* docker stack deploy my-demo-stack-name -c docker-stack.yaml

## How to clean up again
* kubectl delete -f kubernetes.yaml
* docker stack rm my-demo-stack-name
