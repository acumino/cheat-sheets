**Cluster Management:**
- `kubectl version`: Display the Kubernetes client and server version information.
- `kubectl cluster-info`: Display cluster information.
- `kubectl config view`: View the current kubeconfig configuration.
- `kubectl api-resources`: List all the available API resources.
- `kubectl api-versions`: List all the available API versions.
- `kubectl auth can-i <verb> <resource>`: Check if the current user has permission to perform a specific action on a resource.
- `kubectl auth reconcile`: Reconcile the authorization rules for the current user.
- `kubectl cluster-info dump`: Dump the current cluster state to a file.
- `kubectl get events`: List all the events in the cluster.
- `kubectl config get-contexts`: List all available contexts in the kubeconfig.
- `kubectl config use-context <context>`: Set the current context in the kubeconfig.
- `kubectl config use-context <context> --namespace=<namespace>`: Set the current context and default namespace in the kubeconfig.
- `kubectl config set-context <context> --namespace=<namespace>`: Set the default namespace for a context.
- `kubectl get nodes`: List all nodes in the cluster.
- `kubectl describe node <node_name>`: Show detailed information about a specific node.
- `kubectl cordon <node_name>`: Mark a node as unschedulable.
- `kubectl uncordon <node_name>`: Mark a node as schedulable.
- `kubectl drain <node_name>`: Drain a node by evicting all pods gracefully.
- `kubectl taint node <node_name> <taint_key>=<taint_value>:<taint_effect>`: Add a taint to a node.
- `kubectl apply -f <manifest.yaml>`: Apply a manifest to the cluster.
- `kubectl delete -f <manifest.yaml>`: Delete a manifest from the cluster.
- `kubectl edit <resource_type> <resource_name>`: Edit a resource in the cluster.
- `kubectl label <resource_type> <resource_name> <label_key>=<label_value>`: Add a label to a resource.
- `kubectl annotate <resource_type> <resource_name> <annotation_key>=<annotation_value>`: Add an annotation to a resource.

**Namespace Management:**
- `kubectl get namespaces`: List all namespaces in the cluster.
- `kubectl create namespace <namespace_name>`: Create a new namespace.
- `kubectl delete namespace <namespace_name>`: Delete a namespace.
- `kubectl describe namespace <namespace_name>`: Show detailed information about a specific namespace.
- `kubectl apply -f <manifest.yaml>`: Apply a manifest to a specific namespace.
- `kubectl apply -f <manifest.yaml> -n <namespace_name>`: Apply a manifest in a specific namespace.
- `kubectl delete -f <manifest.yaml> -n <namespace_name>`: Delete a manifest from a specific namespace.

**Pod Management:**
- `kubectl get pods`: List all pods in the cluster.
- `kubectl describe pod <pod_name>`: Show detailed information about a specific pod.
- `kubectl create -f <pod_definition.yaml>`: Create a pod from a YAML file.
- `kubectl delete pod <pod_name>`: Delete a pod.
- `kubectl logs <pod_name>`: Display the logs of a pod.
- `kubectl exec -it <pod_name> -- <command>`: Execute a command in a running pod.
- `kubectl port-forward <pod_name> <host_port>:<container_port>`: Forward ports from a pod to the local machine.
- `kubectl attach <pod_name> -c <container_name>`: Attach to a running container in a pod.
- `kubectl cp <pod_name>:<path_to_file> <local_path>`: Copy files between a pod and the local machine.
- `kubectl top pods`: Show resource usage (CPU and memory) of pods.
- `kubectl rollout restart deployment/<deployment_name>`: Restart a deployment by triggering a rollout.
- `kubectl rollout history pod <pod_name>`: View the revision history of a pod.
- `kubectl rollout undo pod <pod_name>`: Roll back a pod to a previous revision.
- `kubectl attach <pod_name>`: Attach to a running container in a pod.
- `kubectl wait pod <pod_name> --for=condition=<condition>`: Wait for a specific condition to be true for a pod.

**Deployment Management:**
- `kubectl get deployments`: List all deployments in the cluster.
- `kubectl describe deployment <deployment_name>`: Show detailed information about a specific deployment.
- `kubectl create -f <deployment_definition.yaml>`: Create a deployment from a YAML file.
- `kubectl delete deployment <deployment_name>`: Delete a deployment.
- `kubectl scale deployment <deployment_name> --replicas=<count>`: Scale a deployment to the specified number of replicas.
- `kubectl rollout status deployment/<deployment_name>`: Check the status of a deployment rollout.
- `kubectl rollout history deployment/<deployment_name>`: View the revision history of a deployment.
- `kubectl rollout history deployment/<deployment_name> --revision=<revision_number>`: View the details of a specific revision of a deployment.
- `kubectl rollout undo deployment/<deployment_name>`: Roll back a deployment to a previous revision.
- `kubectl rollout undo deployment/<deployment_name> --to-revision=<revision_number>`: Roll back a deployment to a specific revision.
- `kubectl rollout pause deployment/<deployment_name>`: Pause a deployment rollout.
- `kubectl rollout resume deployment/<deployment_name>`: Resume a paused deployment rollout.

**Service Management:**
- `kubectl get services`: List all services in the cluster.
- `kubectl describe service <service_name>`: Show detailed information about a specific service.
- `kubectl create -f <service_definition.yaml>`: Create a service from a YAML file.
- `kubectl delete service <service_name>`: Delete a service.

**ConfigMap Management:**
- `kubectl get configmaps`: List all ConfigMaps in the cluster.
- `kubectl describe configmap <configmap_name>`: Show detailed information about a specific ConfigMap.
- `kubectl create configmap <configmap_name> --from-literal=<key>=<value>`: Create a ConfigMap with literal values.
- `kubectl create configmap <configmap_name> --from-file=<path_to_directory>`: Create a ConfigMap from a directory.

**RBAC (Role-Based Access Control) Management**:
- `kubectl create role <role_name> --verb=<verb> --resource=<resource>`: Create a role with specified verbs and resources.
- `kubectl create rolebinding <rolebinding_name> --role=<role_name> --user=<user_name>`: Create a role binding to bind a role to a user.
- `kubectl create clusterrole <clusterrole_name> --verb=<verb> --resource=<resource>`: Create a cluster role with specified verbs and resources.
- `kubectl create clusterrolebinding <clusterrolebinding_name> --clusterrole=<clusterrole_name> --user=<user_name>`: Create a cluster role binding to bind a cluster role to a user.

**Secret Management:**
- `kubectl get secrets`: List all secrets in the cluster.
- `kubectl describe secret <secret_name>`: Show detailed information about a specific secret.
- `kubectl create secret generic <secret_name> --from-literal=<key>=<value>`: Create a secret with literal values.
- `kubectl create secret generic <secret_name> --from-file=<path_to_file>`: Create a secret from a file.

**Ingress Management:**
- `kubectl get ingresses`: List all ingresses in the cluster.
- `kubectl describe ingress <ingress_name>`: Show detailed information about a specific ingress.
- `kubectl create -f <ingress_definition.yaml>`: Create an ingress from a YAML file.
- `kubectl delete ingress <ingress_name>`: Delete an ingress.

**Job and CronJob Management:**
- `kubectl get jobs`: List all jobs in the cluster.
- `kubectl describe job <job_name>`: Show detailed information about a specific job.
- `kubectl create -f <job_definition.yaml>`: Create a job from a YAML file.
- `kubectl delete job <job_name>`: Delete a job.
- `kubectl get cronjobs`: List all cron jobs in the cluster.
- `kubectl describe cronjob <cronjob_name>`: Show detailed information about a specific cron job.
- `kubectl create -f <cronjob_definition.yaml>`: Create a cron job from a YAML file.
- `kubectl delete cronjob <cronjob_name>`: Delete a cron job.
- `kubectl wait job <job_name> --for=condition=<condition>`: Wait for a specific condition to be true for a job.
- `kubectl wait cronjob <cronjob_name> --for=condition=<condition>`: Wait for a specific condition to be true for a cron job.

**Volume Management:**
- `kubectl get pv`: List all persistent volumes in the cluster.
- `kubectl describe pv <persistent_volume_name>`: Show detailed information about a specific persistent volume.
- `kubectl get pvc`: List all persistent volume claims in the cluster.
- `kubectl describe pvc <persistent_volume_claim_name>`: Show detailed information about a specific persistent volume claim.

**ReplicaSet Management:**
- `kubectl get replicasets`: List all ReplicaSets in the cluster.
- `kubectl describe replicasets <replicaset_name>`: Show detailed information about a specific ReplicaSet.
- `kubectl scale replicasets <replicaset_name> --replicas=<count>`: Scale a ReplicaSet to the specified number of replicas.
- `kubectl delete replicasets <replicaset_name>`: Delete a ReplicaSet.
- `kubectl rollout history replicaset <replicaset_name>`: View the revision history of a ReplicaSet.
- `kubectl rollout undo replicaset <replicaset_name>`: Roll back a ReplicaSet to a previous revision.

**StatefulSet Management:**
- `kubectl get statefulsets`: List all StatefulSets in the cluster.
- `kubectl describe statefulset <statefulset_name>`: Show detailed information about a specific StatefulSet.
- `kubectl scale statefulsets <statefulset_name> --replicas=<count>`: Scale a StatefulSet to the specified number of replicas.
- `kubectl delete statefulsets <statefulset_name>`: Delete a StatefulSet.
- `kubectl rollout history statefulset <statefulset_name>`: View the revision history of a StatefulSet.
- `kubectl rollout undo statefulset <statefulset_name>`: Roll back a StatefulSet to a previous revision.

**DaemonSet Management:**
- `kubectl get daemonsets`: List all DaemonSets in the cluster.
- `kubectl describe daemonset <daemonset_name>`: Show detailed information about a specific DaemonSet.
- `kubectl scale daemonsets <daemonset_name> --replicas=<count>`: Scale a DaemonSet to the specified number of replicas.
- `kubectl delete daemonsets <daemonset_name>`: Delete a DaemonSet.
- `kubectl rollout history daemonset <daemonset_name>`: View the revision history of a DaemonSet.
- `kubectl rollout undo daemonset <daemonset_name>`: Roll back a DaemonSet to a previous revision.

**Metrics and Monitoring:**
- `kubectl top nodes`: Show resource usage (CPU and memory) of nodes.
- `kubectl top nodes --sort-by=<resource>`: Show resource usage (CPU and memory) of nodes sorted by a specific resource.
- `kubectl top pods`: Show resource usage (CPU and memory) of pods.
- `kubectl top pods -n <namespace_name>`: Show resource usage (CPU and memory) of pods in a specific namespace.
- `kubectl top pods --sort-by=<resource>`: Show resource usage (CPU and memory) of pods sorted by a specific resource.
