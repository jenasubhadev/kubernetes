# kubernetes

Follow the Steps below - 
## Create the Mongo DB
```
kubectl apply -f mongo.yaml
```

## Create the Config Map
```
kubectl apply -f mongo-configmap.yaml
```
## Create the mongo-express
```
kubectl apply -f mongo-express.yaml
```
If you are running in minikube 
```
minikube service mongo-express-service
```
Else
```
kubectl port-forward service/mongo-express-service 8081:8081
```
