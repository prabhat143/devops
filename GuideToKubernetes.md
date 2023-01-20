# devops wuth k8s

## install hyperkit which is a VM <br>
brew install hyperkit

## install kubernetes
brew install minikube

## To check kubectl commands<br>
kubectl

## To check minikube<br>
minikube

## Create and start the clustor <br>
minikube start --vm-driver=hyperkit <br>
    -- This will install docker into the system. <br>
    
## Get status of the node <br>
kubectl get nodes <br>

## Get minikube status <br>
minikube status
