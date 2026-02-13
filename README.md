- Install the argocd CLI 

- Create nginx namespace: 

```
kubectl create namespace nginx
```

- Deploy nginx app with Argocd

```
argocd app create my-nginx --repo https://github.com/OrlandoSoto/my-argocd-app --path manifests --dest-server https://kubernetes.default.svc --dest-namespace nginx
```

You should see

```
application 'my-nginx' created
```
