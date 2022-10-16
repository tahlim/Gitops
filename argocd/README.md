# Installation process of ArgoCD:
```
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/core-install.yaml
kubectl get all -n argocd
kubectl create clusterrolebinding  tahlimkhan88 --clusterrole=cluster-admin --user=tahlimkhan85@gmail.com
kubectl patch svc argocd-server -n argocd -p '{"spec": {"type": "LoadBalancer"}}'
kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d
```
- user: admin
- password: Mdowv8d6mj-efO0
```
kubectl exec -it argocd-server-895675597-dfq7j -n argocd -- bash

argocd login a13c5890f4330432690751d2b4e717f1-915922224.us-east-1.elb.amazonaws.com

argocd account update-password
```
```
kubectl delete -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/core-install.yaml
kubectl delete -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
```
