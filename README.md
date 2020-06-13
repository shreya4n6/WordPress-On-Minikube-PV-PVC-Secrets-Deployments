# WordPress-On-Minikube-PV-PVC-Secrets-Deployments

TL; DR

Installing WordPress On Kubernetes.

1. We will create a persistent volume (PV) for both our MySQL & WordPress Pods followed by persistent volume claims (PVC) for the same.
2. Creating A Secret Of MySQL Root Password followed by Deployment of MySQL:5.6 Pod & Attaching MySQL Volume created above.
3. Exposing Deployment with Service Type ClusterIP
4. Creating A Deployment Of WordPress:4.8-apache Pod, Attaching the Volumes & Putting Database Details Using Environment variables.
5. Exposing WordPress Deployment with Service Type NodePort

Prerequisites

Minikube Installed
Kubectl configured with Minikube
