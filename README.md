Kubernetes with Persistent Volumes and Docker Compose

This repository contains files and configurations to deploy Kubernetes resources with persistent volumes, using Docker and Docker Compose. It includes deployment and service YAML files, persistent volume (PV) and persistent volume claim (PVC) definitions, and environment variables for managing file writes.

Project Overview

The goal of this project is to demonstrate how to persist data in Kubernetes using Docker volumes and compose files. By leveraging persistent volumes and claims, the application can retain data even after pods are terminated.

Directory Structure
/
|-- docker-compose.yaml
|-- k8s/
|   |-- deployment.yaml
|   |-- service.yaml
|   |-- persistent-volume.yaml
|   |-- persistent-volume-claim.yaml
|-- .env
|-- README.md

kubectl apply -f vol_persist.yaml
kubectl apply -f vol_persistclaim.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml


 Verify Deployments and Services
 kubectl get pods
kubectl get services
