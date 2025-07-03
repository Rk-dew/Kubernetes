eksctl create cluster --config-file=eks.yaml # Creates cluster

kubectl create namespace # Create a namespace

kubectl create deployment --image= # Create a deployment

kubectl create service clusterip --tcp=80:80 # Create a ClusterIP service

kubectl create service nodeport --tcp=80:80 # Create a NodePort service

kubectl create configmap --from-literal=key=value # Create config map from literal

kubectl apply -f <file.yaml>

kubectl delete -f <file.yaml>

kubectl get pods # List all pods

kubectl get svc # List all services

kubectl get deployments # List all deployments

kubectl get rs # List all replica sets

kubectl get nodes # List all nodes in the cluster

kubectl get namespaces # List all namespaces

kubectl get configmaps # List all config maps

kubectl get secrets # List all secrets

kubectl get pods -n # Pods in specific namespace

kubectl get all -n # All resources in specific namespace

kubectl describe pod # Describe a pod

kubectl describe deployment # Describe a deployment

kubectl describe svc # Describe a service

kubectl describe configmap # Describe a config map

kubectl describe secret # Describe a secret

kubectl describe node

kubectl exec -it <pod_name> -- bash # Opens an interactive shell (bash) inside a running pod.

alias ka='kubectl apply -f' # If we run this command we can simply write 'ka' in place of 'kubectl apply -f'

kubectl delete pod # Delete a specific pod

kubectl delete deployment # Delete a specific deployment

kubectl delete svc # Delete a service

kubectl delete configmap # Delete a config map

kubectl delete secret # Delete a secret

kubectl delete node # Delete a node (from cluster)

kubectl delete namespace # Delete a namespace

eksctl delete cluster <cluster_name>

eksctl delete cluster --config-file=eks.yaml
