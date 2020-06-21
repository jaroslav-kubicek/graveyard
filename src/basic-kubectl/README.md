# Kubernetes basics

Ho to run in `minikube`:

1. Build docker image into `minikube`

```
eval $(minikube docker-env)
docker build src/basic-kubectl --tag basic-kubectl
```

2. Run deployment

```
kubectl apply -f src/basic-kubectl/.K8s/basicKustomize.yaml
kubectl expose deployment hello.world --type=NodePort --name=hello
minikube service hello --url
```
