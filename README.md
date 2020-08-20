# Using Volume with SBR

```
export KUBECONFIG=</path/to/kubeconfig>
kubectl apply -f backend-crd-volumemount.yaml
kubectl apply -f backend-cr.yaml
kubectl apply -f app-crd.yaml
kubectl apply -f app-cr.yaml
kubectl apply -f sbr.yaml
```

Now run `make local` from SBR codebase.

Check the appconfig:

```
kubectl get appconfig  demo-appconfig -o yaml
```

