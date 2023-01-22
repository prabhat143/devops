# devops

Deployemnt manages replicaset <br>
replicaset manages pod <br>
pod is an abstraction of containers. <br>

Everything below the deplyment is handled by kubernetes

## Edit deployment name <bro>
kubectl edit deployment nginx-depl
      -- this will give an Auto-generated configuration file with default values

## logs in k8s<bro>
kubectl logs [pod name]  
      
## Install mongo db<bro>
kubectl create deployment mongo-depl --image=mongo      
      
## Describe a pod
kubectl describe pod [pod name] <br>
      Sample O/P <br>
      Events: <br>
  Type    Reason     Age    From               Message <br>
  ----    ------     ----   ----               ------- <br>
  Normal  Scheduled  3m55s  default-scheduler  Successfully assigned default/mongo-depl-8fbdb868c-4b946 to minikube<br>
  Normal  Pulling    3m55s  kubelet            Pulling image "mongo" <br>
  Normal  Pulled     3m21s  kubelet            Successfully pulled image "mongo" in 33.65748325s<br>
  Normal  Created    3m21s  kubelet            Created container mongo<br>
  Normal  Started    3m21s  kubelet            Started container mongo<br>
      
 
# To create a Interactive Terminal(-it) for specific pod <br>
kubectl exec -it [pod name] -- bin/bash <br>
    
#Delete deployment
kubectl delete deployment [deployment name] <br>
      
#Apply configuration  - in practice you use configuration file rather commands to execute kuberntes
kubectl apply -f [configuration file name] <br>
      example kubectl apply -f config-file.yml <br>
      
