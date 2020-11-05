# kubernetes-beginning
Kubernetes with docker


# commnad to run both file through kubectl
kubectl apply -f ./client.pod.yml
kubectl apply -f ./client-network.yml

# command to get both objects/config
kubectl get pods
kubectl get services
- extra information of objects
kubectl get pods -o wide

# command to inspect pods what containers/image is running inside it
kubectl describe <objecttype> <objectname>
kubectl describe pod client-pod

# pod restriction
Through pod config file, we can not update containers, name, port except image
kubernetes porvides another type of object type <Deployment>


# remove existing objects
kubectl delete -f client-pod

# connecting to Minikube with browser
minikube ip

# forcefully tell kubectl to use latest version of image from dockerhub
kubectl set image <object type> / <object name> <container name> = <new image to use>
kubectl set image deployment/client-deployment client = apurwar15/multiclient:v5


 