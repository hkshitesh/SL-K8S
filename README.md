# Multi-container commands
kubectl exec -it multi-container-pod -c logger-container -- /bin/sh

kubectl exec -it multi-container-pod -c nginx-container -- /bin/bash

# container log
kubectl logs multi-container-pod -c nginx-container

kubectl logs multi-container-pod -c logger-container

# etcd command

sudo ETCDCTL_API=3 etcdctl --endpoints $advertise_url --cacert /etc/kubernetes/pki/etcd/ca.crt --key /etc/kubernetes/pki/etcd/server.key --cert /etc/kubernetes/pki/etcd/server.crt snapshot save etcd_backup.db


## Azure Cloud Shell

az account set --subscription 2f02f8ca-866d-410a-bfed-32876b28bc58

az aks get-credentials --resource-group Regroup_6tK8WPlWWd1ajy24YTj-vnet --name SL-Cluster
