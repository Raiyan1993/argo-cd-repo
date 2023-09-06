# argo-cd-repo

**Pre-requisite:**

1. Create EKS Cluster [here](https://github.com/Raiyan1993/terraform/tree/master/EKS-project-1)
2. Install Argo CD by [reference](https://argo-cd.readthedocs.io/en/stable/getting_started/)
~~~
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
~~~

**Port Forwarding¶**

Kubectl port-forwarding can also be used to connect to the API server without exposing the service.
~~~
kubectl port-forward svc/argocd-server -n argocd 8080:443
~~~

The API server can then be accessed using https://localhost:8080
