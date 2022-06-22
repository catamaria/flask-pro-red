# flask-pro-red
flask service using redis as cache and postgress as db in kubernetes

# sources
https://loft.sh/blog/docker-compose-to-kubernetes-step-by-step-migration/
https://minikube.sigs.k8s.io/docs/tutorials/multi_node/


## To run project locally 

1) > cd flask-pro-red
2) > minikube start -p node
3) > skaffold run --port-forward --tail


## In case the image is running locally --ignore for now since its in my hub
> cd flask-pro-red
>  
> sudo docker-compose up -d --build


To use this command you can follow the instructions from here
https://skaffold.dev/docs/install/

### not necessary since the yaml files are already created 
>skaffold init --compose-file docker-compose.yaml

