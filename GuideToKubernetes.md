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

## Get minikube status <br>
minikube status

## Kubectl cli purpose<br>
For configring the MiniKube CLuster

## minikube cli purpose<br>
For start up/deleting the cluster

## CRUD commands<br>
create deployement -> kubecli create deployment [name]
Edit deployment -> kubecli edit deployment [name]
delete deployment -> kubecli delete deployment [name]

## Status of different k8s componnents<br>
kubecli get nodes | pod | services | replicaset | deployment

## Debugging pods<br>
log to consile -> kubecli logs [pod name]
get Interactive Terminal -> kubel exec -it [pod name] -- bin/bash


