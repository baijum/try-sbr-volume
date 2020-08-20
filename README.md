# Using Volume with SBR

using a custom resource:

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

using a deployment:

```
export KUBECONFIG=</path/to/kubeconfig>
kubectl apply -f backend-crd-volumemount.yaml
kubectl apply -f backend-cr.yaml
kubectl apply -f app-deployment.yaml
kubectl apply -f sbr-deployment.yaml
```

Now run `make local` from SBR codebase.

Check the appconfig:

```
kubectl get appconfig  demo-appconfig -o yaml
```
