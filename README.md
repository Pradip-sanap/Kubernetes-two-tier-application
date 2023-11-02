# Kubernetes-two-tier-application
Deploying two tier application with kubenetes. Mongo-Express as UI and mongoDb as database.
Manifest files are create for deployment.

We use minikube to deploy application.

Commands for deployment:
kubectl apply -f mongo-app.yaml

kubectl apply -f mongo-config.yaml

kubectl apply -f secret.yaml

kubectl apply -f .\web-app.yaml 

## check 
kubectl get pods 
kubectl get svc
kubectl get all

## We had create service for both webapp and database. We need to expose service to outer world. In minikube, it done using command.
minikube service webapp-service

## Default username and password for alert box is "admin" and "pass" respectively. It is by default for mongo-express.

Mongo-Express: It is UI given for user to easily add, delete and manipulate databases in mongoDb.
