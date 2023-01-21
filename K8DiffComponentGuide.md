# Get status of different components

pre- requests:
    - minikube installled
    - kubectl installed

## get status of the node <br>
kubectl get nodes

## get status of the pod <br>
kubectl get pod

## get status of the services <br>
kubectl get services

## create a pod <br>
In k8 world pod is the smallest unit. but you are creating deployment - absraction over pod
Usage:<br>
   kubectl create deployment NAME --image=image [--dry-run] [options]<br>
   example : kubectl create deployment nginx-depl --image=nginx
   
## Get replicaset <br>   
kubectl get replicaset  

#### NOTE: if you want number of replicas on pod the we need to use [option] while create the deployment.
