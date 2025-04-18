# kubestellar-ui-charts
I also created Helm charts for Kubestellar UI, but the issue persists there as well.
Helm commands I used:
```
helm repo add kubestellar-ui https://mavrick-1.github.io/kubestellar-ui/
helm repo update
helm install kubestellar-ui kubestellar-ui/kubestellar-ui
```
Port-forwarding commands:
```
kubectl port-forward svc/frontend 5173:80 -n default
kubectl port-forward svc/backend 4000:4000 -n default
```
[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/kubestellar-ui)](https://artifacthub.io/packages/search?repo=kubestellar-ui)