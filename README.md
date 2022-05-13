# minikube-jenkins

```
kubectl create ns jenkins
kubectl apply -f jenkins-sc.yaml
kubectl apply -f jenkins-volume.yaml
kubectl apply -f jenkins-sa.yaml

helm install jenkins ./jenkins/ --namespace jenkins
```

#IMPORTANT! After succesfull install remove this block with init container from StatefulSet.
