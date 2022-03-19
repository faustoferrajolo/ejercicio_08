# Ejercicio 8
## Despliegue de password-api

### Comandos

```sh
kubectl create namespace pass-api
kubectl apply -f deployment-ej8.yaml
kubectl apply -f service-ej8.yaml -n pass-api
minikube ip
curl 192.168.49.2:30796
kubectl port-forward svc/pass-api -n pass-api 3000:3000 --address='0.0.0.0'
```
### Web Browser
 - localhost:3000
