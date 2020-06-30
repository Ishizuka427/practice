## NGINX Ingress Controllerのインストール

参照: [Installation Guide - NGINX Ingress Controller](https://kubernetes.github.io/ingress-nginx/deploy/)

Docker for Macの場合


```sh
$ kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/master/deploy/static/provider/cloud/deploy.yaml
```

インストールできたか確認

```sh
$ kubectl get pods -n ingress-nginx \
  -l app.kubernetes.io/name=ingress-nginx --watch
```

