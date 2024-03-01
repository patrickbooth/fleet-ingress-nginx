# fleet-ingress-nginx
Fleet gitrepo for ingress-nginx

### Install Fleet via Helm

```
$ helm repo add fleet https://rancher.github.io/fleet-helm-charts/
$ helm -n fleet-system install --create-namespace --wait fleet-crd fleet/fleet-crd
$ helm -n fleet-system install --create-namespace --wait fleet fleet/fleet
```

