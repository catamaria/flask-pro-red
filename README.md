# flask-pro-red
flask service using redis as cache and postgress as db in kubernetes

# sources
https://loft.sh/blog/docker-compose-to-kubernetes-step-by-step-migration/
https://minikube.sigs.k8s.io/docs/tutorials/multi_node/

# test docker

kubectl create -f web-service.yaml


> cd flask-pro-red
>  
> sudo docker-compose up -d --build


## add nodes to minicukube

>minikube start -p node2
>
>minikube start -p node3

## convert to kubernetes
To use this command you can follow the instructions from here
https://skaffold.dev/docs/install/

>skaffold init --compose-file docker-compose.yaml

## run with logs 
>skaffold run --port-forward --tail

