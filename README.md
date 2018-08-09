# Kubernetes-Prometheus

Steps to create a kubernetes cluster
```
#install kubeadm
#follow instructions from https://kubernetes.io/docs/setup/independent/install-kubeadm/
#create a cluster
#follow instructions on https://kubernetes.io/docs/setup/independent/create-cluster-kubeadm/
```
To setup monitoring architecture with Prometheus and Graphana
```
kubectl create namespace monitoring

kubectl apply -f prometheus-config.yaml

kubectl apply -f cluster-role.yaml

kubectl apply -f service-account.yaml

kubectl apply -f cluster-role-binding.yaml

kubectl apply -f prometheus-deployment.yaml

kubectl apply -f prometheus-service.yaml

kubectl apply -f grafana-deployment.yaml

kubectl apply -f grafana-service.yaml
```
