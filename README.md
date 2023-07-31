argocd admin initial-password -n argocd

## ArgoCD control interface (localhost:8080)
kubectl port-forward svc/argocd-server -n argocd 8080:443 

## Wealthy backend (localhost:9090)
kubectl port-forward svc/wealthy-backend 9090:80

## Wealthy Postgress DB (localhost:9091)
kubectl port-forward svc/wealthy-db 9091:5432