# devops-assignment
Assignment for creating  a complete CI/CD infrastructure pipeline on AWS using Terraform, Kubernetes, ArgoCD.

This repository contains the code and configuration I used to build a complete CI/CD setup on AWS using Terraform, EKS, Kubernetes, and ArgoCD.

The setup provisions an EKS cluster, deploys an NGINX application, and uses ArgoCD for GitOps based continuous delivery.

This application is exposed through an Ingress controller with a DNS hostname(http://mydemonginx.nosky.io/).


1. Infrastructure – Terraform (EKS Cluster)

All Terraform files are under the terraform/ folder.

The Terraform setup does the following:

Creates a dedicated VPC

Deploys an EKS cluster (1.30)

Creates a managed node group

Outputs cluster endpoint and cluster name

Generates kubeconfig for connecting to the cluster

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/7575d57f-0ab1-4627-8888-a8eb310535e1" />





