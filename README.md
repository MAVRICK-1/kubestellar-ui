# kubestellar-ui-charts
I also created Helm charts for Kubestellar UI, but the issue persists there as well.
Helm commands I used:
```
helm repo add kubestellar-ui https://mavrick-1.github.io/kubestellar-ui/
helm repo update
helm install kubestellar-ui kubestellar-ui/kubestellar-ui --set kubeConfig="$( cat ~/.kube/config )"
```
Port-forwarding commands:
```
kubectl port-forward svc/frontend 8080:80 -n default
kubectl port-forward svc/backend 4000:4000 -n default
```
