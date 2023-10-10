# Kubernetes do Zero à Produção

K8S = Kubernetes => Orquestrador de Containers
Necessita de um container run time => Docker

Instalar o kubectl e o kind 

https://kind.sigs.k8s.io/docs/user/quick-start/

## Create a cluster 
kind create cluster --name=esquenta

## Delete a cluster
kind delete cluster --name=esquenta

kubectl cluster-info –contect kind-esquenta
kubectl get nodes

kubectl apply -f k8s/pod.yaml
kubectl delete pod nginx


kubectl get pods

kubectl port-forward pod/nginx 8089:80
kubectl port-forward --address 0.0.0.0 pod/nginx 8089:80

kubectl get rs

kubectl get svc

Para AWS 

Gerado o kubeconfig

cp kubeconfig ~./kubeconfig

kubectl get nodes

retorna kubernetes da AWS
 