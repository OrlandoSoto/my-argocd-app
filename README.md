Install the argocd CLI then run:
`argocd app create my-nginx --repo https://github.com/OrlandoSoto/my-argocd-app --path manifests --dest-server https://kubernetes.default.svc --dest-namespace nginx`

You should see

```
application 'my-nginx' created
```
