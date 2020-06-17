## Docker

#### condensed docker ps

```docker ps --format "table {{.ID}}\t{{.Names}}\t{{.Status}}"```

## K8s

#### interactive k8s pod
```kubectl run my-pod --restart=Never -it --rm --image ubuntu -- bash```

#### accessx API via curl in a pod 
```
curl -k \
  -H "Authorization: Bearer $(cat /run/secrets/kubernetes.io/serviceaccount/token)" \
  https://172.20.0.1/api/v1/namespaces/szde/pods/`
```