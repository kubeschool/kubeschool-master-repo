# Installation

This folder includes Kubernetes manifests for installing NGINX or NGINX Plus Ingress controller. Read the installation instructions [here](https://docs.nginx.com/nginx-ingress-controller/installation/).


kubectl config use-context EricDewhirst@kubeschool.us-east-1.eksctl.io 

kubectl apply -f common/ns-and-sa.yaml
kubectl apply -f common/default-server-secret.yaml
kubectl apply -f common/nginx-config.yaml
kubectl apply -f rbac/rbac.yaml
kubectl apply -f common/ingress-class.yaml
kubectl apply -f deployment/nginx-ingress.yaml
kubectl apply -f service/loadbalancer-aws-elb.yaml


