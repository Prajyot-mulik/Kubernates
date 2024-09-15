# Kubernetes Pods and Services Commands

## Pod Management
- `kubectl get pods`          ----- List all pods in the current namespace
- `kubectl get pods --all-namespaces` ----- List all pods across all namespaces
- `kubectl describe pod <pod_name>` ----- Get detailed information about a pod
- `kubectl logs <pod_name>`   ----- Print logs of a pod
- `kubectl exec -it <pod_name> -- /bin/bash` ----- Access a running pod's shell
- `kubectl delete pod <pod_name>` ----- Delete a pod

## Service Management
- `kubectl get services`      ----- List all services
- `kubectl describe service <service_name>` ----- Describe a service
- `kubectl expose deployment <deployment_name> --type=<service_type> --port=<port>` ----- Expose a deployment as a service
- `kubectl delete service <service_name>` ----- Delete a service

## Port Forwarding
- `kubectl port-forward <pod_name> <local_port>:<remote_port>` ----- Forward a port from a pod to your local machine
