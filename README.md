# Multi-container commands
kubectl exec -it multi-container-pod -c logger-container -- /bin/sh

kubectl exec -it multi-container-pod -c nginx-container -- /bin/bash

# container log
kubectl logs multi-container-pod -c nginx-container

kubectl logs multi-container-pod -c logger-container
