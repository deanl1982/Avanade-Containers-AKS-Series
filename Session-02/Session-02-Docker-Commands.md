# Session 02
## Deploying Containers in AKS

**Login to Tenant and ACR**

'az login --tenant [tenant-id]'
'az acr login --name [contsess02]'

**Tag and push container image to ACR**

'docker tag [docker-image-name-here] [contsess02].azurecr.io/[docker-image-name-here]:latest'
'docker push [contsess02].azurecr.io/[docker-image-name-here]:latest'

**Connect to AKS**

'az aks get-credentials --resource-group [rg-name-here] --name [aks-instance-name-here]'

**Deploy K8s Manifests**

'kubectl apply -f web-app-fe.yml'

'kubectl apply -f web-app-fe-service.yml'

**Useful K8s Kubectl Commands**

'kubectl get deployments --all-namespaces'
'kubectl get pods --all-namespaces'
'kubectl get nodes --all-namespaces'
'kubectl get services'