# HELM COMMANDS REFERENCE
## Basic Commands
- helm repo
- helm search
- helm install
- helm uninstall
- helm list

## Repos Management
- **List Repos**
  ```
  helm repo list
  ```
- **Add repo**
  ```
  helm repo add <NAME> <URL>
  helm repo add mybitnami https://charts.bitnami.com/bitnami
  ```
- **Search repo**
```
# Search for nginx in all configured repos
helm search repo nginx

# List all versions of nginx
helm search repo nginx --versions

# List repo with specific version
helm search repo nginx --version 11.2.1
```
- **Install and Uninstall**
```
# Install 
helm install mynginx mybitnami/nginx

# UnInstall
helm uninstall mynginx
```
