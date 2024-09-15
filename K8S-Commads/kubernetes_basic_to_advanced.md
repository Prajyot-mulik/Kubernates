# Kubernetes Basic to Advanced Commands

## Cluster Information
- `kubectl cluster-info`      ----- Displays cluster info
- `kubectl get nodes`         ----- List all nodes in the cluster
- `kubectl describe node <node_name>` ----- Describe a node

## Namespace Management
- `kubectl get namespaces`    ----- List all namespaces
- `kubectl create namespace <namespace_name>` ----- Create a namespace
- `kubectl delete namespace <namespace_name>` ----- Delete a namespace
- `kubectl config set-context --current --namespace=<namespace_name>` ----- Switch to a namespace

## Pod Management
- `kubectl get pods`          ----- List all pods in the current namespace
- `kubectl get pods --all-namespaces` ----- List all pods across all namespaces
- `kubectl describe pod <pod_name>` ----- Get detailed information about a pod
- `kubectl logs <pod_name>`   ----- Print logs of a pod
- `kubectl exec -it <pod_name> -- /bin/bash` ----- Access a running pod's shell

## Deployment Management
- `kubectl create deployment <name> --image=<image_name>` ----- Create a deployment
- `kubectl get deployments`  ----- List deployments
- `kubectl describe deployment <deployment_name>` ----- Describe a deployment
- `kubectl scale deployment <deployment_name> --replicas=<number>` ----- Scale a deployment

## Service Management
- `kubectl get services`      ----- List all services
- `kubectl describe service <service_name>` ----- Describe a service
- `kubectl expose deployment <deployment_name> --type=<service_type> --port=<port>` ----- Expose a deployment as a service

## ConfigMaps and Secrets
- `kubectl get configmaps`    ----- List all ConfigMaps
- `kubectl describe configmap <configmap_name>` ----- Describe a ConfigMap
- `kubectl get secrets`      ----- List all secrets
- `kubectl describe secret <secret_name>` ----- Describe a secret

## Volumes and Persistent Volumes
- `kubectl get pv`            ----- List all persistent volumes
- `kubectl get pvc`           ----- List all persistent volume claims
- `kubectl describe pv <pv_name>` ----- Describe a persistent volume
- `kubectl describe pvc <pvc_name>` ----- Describe a persistent volume claim

## Advanced Commands
- `kubectl apply -f <file.yaml>` ----- Apply a configuration from a file
- `kubectl delete -f <file.yaml>` ----- Delete resources defined in a file
- `kubectl top pod`            ----- Show resource usage (requires metrics-server)
- `kubectl rollout status deployment/<deployment_name>` ----- Check rollout status of a deployment
- `kubectl port-forward <pod_name> <local_port>:<remote_port>` ----- Forward a port from a pod to your local machine

## Helm Commands
- `helm install <release_name> <chart>` ----- Install a Helm chart
- `helm upgrade <release_name> <chart>` ----- Upgrade a Helm release
- `helm list`                 ----- List all Helm releases
- `helm delete <release_name>` ----- Delete a Helm release
