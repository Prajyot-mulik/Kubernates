# Kubernetes Objects Commands

## Deployments
- `kubectl get deployments`  ----- List deployments
- `kubectl describe deployment <deployment_name>` ----- Describe a deployment
- `kubectl delete deployment <deployment_name>` ----- Delete a deployment
- `kubectl rollout status deployment/<deployment_name>` ----- Check rollout status of a deployment

## ReplicaSets
- `kubectl get replicasets`  ----- List ReplicaSets
- `kubectl describe replicaset <replicaset_name>` ----- Describe a ReplicaSet
- `kubectl delete replicaset <replicaset_name>` ----- Delete a ReplicaSet

## StatefulSets
- `kubectl get statefulsets`  ----- List StatefulSets
- `kubectl describe statefulset <statefulset_name>` ----- Describe a StatefulSet
- `kubectl delete statefulset <statefulset_name>` ----- Delete a StatefulSet

## DaemonSets
- `kubectl get daemonsets`   ----- List DaemonSets
- `kubectl describe daemonset <daemonset_name>` ----- Describe a DaemonSet
- `kubectl delete daemonset <daemonset_name>` ----- Delete a DaemonSet

## Jobs
- `kubectl get jobs`         ----- List Jobs
- `kubectl describe job <job_name>` ----- Describe a Job
- `kubectl delete job <job_name>` ----- Delete a Job

## CronJobs
- `kubectl get cronjobs`     ----- List CronJobs
- `kubectl describe cronjob <cronjob_name>` ----- Describe a CronJob
- `kubectl delete cronjob <cronjob_name>` ----- Delete a CronJob

# Kubernetes ConfigMaps and Secrets Commands

## ConfigMaps
- `kubectl get configmaps`    ----- List all ConfigMaps
- `kubectl describe configmap <configmap_name>` ----- Describe a ConfigMap
- `kubectl create configmap <configmap_name> --from-literal=<key>=<value>` ----- Create a ConfigMap from literal values
- `kubectl delete configmap <configmap_name>` ----- Delete a ConfigMap

## Secrets
- `kubectl get secrets`      ----- List all Secrets
- `kubectl describe secret <secret_name>` ----- Describe a Secret
- `kubectl create secret generic <secret_name> --from-literal=<key>=<value>` ----- Create a Secret from literal values
- `kubectl delete secret <secret_name>` ----- Delete a Secret


# Kubernetes Volumes and Persistent Volumes Commands

## Persistent Volumes (PV)
- `kubectl get pv`            ----- List all Persistent Volumes
- `kubectl describe pv <pv_name>` ----- Describe a Persistent Volume
- `kubectl delete pv <pv_name>` ----- Delete a Persistent Volume

## Persistent Volume Claims (PVC)
- `kubectl get pvc`           ----- List all Persistent Volume Claims
- `kubectl describe pvc <pvc_name>` ----- Describe a Persistent Volume Claim
- `kubectl delete pvc <pvc_name>` ----- Delete a Persistent Volume Claim

## Storage Classes
- `kubectl get storageclasses`  ----- List all Storage Classes
- `kubectl describe storageclass <storageclass_name>` ----- Describe a Storage Class
- `kubectl delete storageclass <storageclass_name>` ----- Delete a Storage Class

# Kubernetes Ingress and Network Policies Commands

## Ingress
- `kubectl get ingress`        ----- List all Ingress resources
- `kubectl describe ingress <ingress_name>` ----- Describe an Ingress resource
- `kubectl delete ingress <ingress_name>` ----- Delete an Ingress resource

## Network Policies
- `kubectl get networkpolicies` ----- List all Network Policies
- `kubectl describe networkpolicy <network_policy_name>` ----- Describe a Network Policy
- `kubectl delete networkpolicy <network_policy_name>` ----- Delete a Network Policy


# Kubernetes Namespaces and Resource Quotas Commands

## Namespaces
- `kubectl get namespaces`    ----- List all namespaces
- `kubectl describe namespace <namespace_name>` ----- Describe a namespace
- `kubectl delete namespace <namespace_name>` ----- Delete a namespace

## Resource Quotas
- `kubectl get resourcequotas` ----- List all Resource Quotas
- `kubectl describe resourcequota <resourcequota_name>` ----- Describe a Resource Quota
- `kubectl delete resourcequota <resourcequota_name>` ----- Delete a Resource Quota


# Kubernetes Custom Resource Definitions (CRDs) and Custom Resources Commands

## Custom Resource Definitions (CRDs)
- `kubectl get crds`            ----- List all Custom Resource Definitions
- `kubectl describe crd <crd_name>` ----- Describe a Custom Resource Definition
- `kubectl delete crd <crd_name>` ----- Delete a Custom Resource Definition

## Custom Resources
- `kubectl get <custom_resource_plural>` ----- List all custom resources of a specific type
- `kubectl describe <custom_resource_plural> <resource_name>` ----- Describe a custom resource
- `kubectl delete <custom_resource_plural> <resource_name>` ----- Delete a custom resource
