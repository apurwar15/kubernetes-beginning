# kubernetes-beginning
Kubernetes with docker


# commnad to run both file through kubectl
kubectl apply -f ./client.pod.yml
kubectl apply -f ./client-network.yml

# command to get both objects/config
kubectl get pods
kubectl get services

# command to inspect pods what containers/image is running inside it
kubectl describe <objecttype> <objectname>
kubectl describe pod client-pod

# pod restriction
Through pod config file, we can not update containers, name, port except image
kubernetes porvides another type of object type <Deployment>


# remove existing objects
kubectl delete -f client-pod
 