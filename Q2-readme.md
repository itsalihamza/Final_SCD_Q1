Namespace
kubectl create namespace 22i-2566-mern-app

Create the namespace for your MERN app.
kubectl get ns

Verify namespace exists.

Deployments
kubectl apply -f frontend-deployment.yaml
kubectl apply -f backend-deployment.yaml
kubectl apply -f mongodb-deployment.yaml

Deploy the frontend, backend, and MongoDB.



kubectl get deployments -n 22i-2566-mern-app

Check that deployments are running.


Pods
kubectl get pods -n 22i-2566-mern-app


Services
kubectl get svc -n 22i-2566-mern-app

List frontend, backend, and MongoDB services.
s.

Cleanup / Restart
kubectl delete pod <pod-name> -n 22i-2566-mern-app

Delete problematic pod to force restart.
kubectl get all -n 22i-2566-mern-app

Quick overview of all resources in the namespace.
