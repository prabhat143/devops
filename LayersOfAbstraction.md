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
kubectl describe pod [pod name]
      Sample O/P
      Events:
  Type    Reason     Age    From               Message
  ----    ------     ----   ----               -------
  Normal  Scheduled  3m55s  default-scheduler  Successfully assigned default/mongo-depl-8fbdb868c-4b946 to minikube
  Normal  Pulling    3m55s  kubelet            Pulling image "mongo"
  Normal  Pulled     3m21s  kubelet            Successfully pulled image "mongo" in 33.65748325s
  Normal  Created    3m21s  kubelet            Created container mongo
  Normal  Started    3m21s  kubelet            Started container mongo

      
