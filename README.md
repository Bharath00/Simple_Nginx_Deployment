# Simple_Nginx_Deployment

Simple Nginx deployment using Kubernetes and Minikube

Required: Docker, Kubernetes, kubectl, minikube

Check if minikube is up and running by using "minikube status" if not then start minikube by using "minikube start"

Note: Services of type LoadBalancer can be exposed via the "minikube tunnel" command. It must be run in a separate terminal window to keep the LoadBalancer running (https://minikube.sigs.k8s.io/docs/handbook/accessing/)

*) kubectl apply -f nginx-deployment.yaml

*) kubectl get svc

The service created is "nginx-service". 
Note that without minikube tunnel, kubernetes would be showing external IP as “pending”. 

*) Copy the url and replace the external ip with your external ip.  http://REPLACE_WITH_EXTERNAL_IP:8080
