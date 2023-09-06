# argo-cd-repo

**Pre-requisite:**

1. Create EKS Cluster [here](https://github.com/Raiyan1993/terraform/tree/master/EKS-project-1)
2. Install Argo CD by [reference](https://argo-cd.readthedocs.io/en/stable/getting_started/)
~~~
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
~~~
