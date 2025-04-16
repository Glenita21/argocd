# Term Project 2025

## Team Contributors:

- **Aafrin Naaz** (C0929235)  
- **Glenita Shareen Furtado** (C0924636)  
- **Pranjal Sankhe** (C0928934)  
- **Manasi Koli** (C0929076)  

---

## Install Helm on Windows

To install Helm on Windows, use the following command:
```
choco install kubernetes-helm
```

## Create helm charts
```
helm create frontend
helm create backend
```

## Yaml files created
```
deployment.yaml
services.yaml
configmap.yaml
secrets.yaml
dev/values.yaml
dev/secrets.yaml
chart.yaml
```
## Deploy app
Go to frontend folder and execute:
```
helm install frontend-app -n frontend . -f dev/values.yaml -f dev/secrets.yaml
```
Go to backend folder and execute:
```
helm install backend-app -n backend . -f dev/values.yaml -f dev/secrets.yaml
```

## To uninstall
```
helm uninstall wordpress-db -n wpdb
helm uninstall wordpress-app -n wpapp
```