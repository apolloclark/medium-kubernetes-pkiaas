# vault-pki-aws-eks-nginx

This repo is forked from the origianl [medium-kubernetes-pkiaas git repo](https://github.com/nehrman/medium-kubernetes-pkiaas) and [Medium article](https://medium.com/hashicorp-engineering/securing-k8s-ingress-traffic-with-hashicorp-vault-pkiaas-and-jetstack-cert-manager-cb46195742ca)) written by [Nicolas Ehrman (Staff Solutions Engineer at HashiCorp)](https://www.linkedin.com/in/nicolas-ehrman-629b8910/), published on 2020-04-07. This proof-of-concept (PoC) / demo repo shows how to use [HashiCorp Vault](https://www.vaultproject.io/), using the [Vault - K8S Auth Method](https://www.vaultproject.io/docs/auth/kubernetes) and [Vault - PKI Secrets Engine](https://www.vaultproject.io/api-docs/secret/pki), within [AWS EKS](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html) / K8S cluster, with an [NGINX Ingress Controller](https://docs.nginx.com/nginx-ingress-controller/), to dynamically generate and rotate TLS certs with the [JetStack cert-manager](https://cert-manager.io/docs/), using [HashiCorp Terraform](https://www.terraform.io/), and the [Terraform - Vault Provider](https://registry.terraform.io/providers/hashicorp/vault/latest/docs).

Changes:
- added AWS EKS
- added an AWS EC2-based Vault Server

Links:
- [Securing K8s Ingress Traffic with HashiCorp Vault PKIaaS and JetStack Cert-Manager](https://medium.com/hashicorp-engineering/securing-k8s-ingress-traffic-with-hashicorp-vault-pkiaas-and-jetstack-cert-manager-cb46195742ca)
- [HashiCorp Vault](https://www.vaultproject.io/)
- [Vault - K8S Auth Method](https://www.vaultproject.io/docs/auth/kubernetes)
- [Vault - PKI Secrets Engine](https://www.vaultproject.io/api-docs/secret/pki)
- [What is Amazon EKS?](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html)
- [Kubernetes Ingress](https://kubernetes.io/docs/concepts/services-networking/ingress)
- [NGINX Ingress Controller - Github](https://github.com/kubernetes/ingress-nginx)
- [cert-manager](https://cert-manager.io/docs/)
- [HashiCorp Terraform](https://www.terraform.io/)
- [Terraform - Vault Provider](https://registry.terraform.io/providers/hashicorp/vault/latest/docs)



## Install

```shell
git clone https://github.com/apolloclark/vault-pki-aws-eks-nginx
cd ./vault-pki-aws-eks-nginx

# verify that you have AWS access
aws sts get-caller-identity

# terraform
terraform init
terraform validate
terraform fmt
terraform plan
terraform apply
```



## Debug
```shell

```
