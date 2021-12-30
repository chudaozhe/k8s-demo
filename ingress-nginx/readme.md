# 准备
## 下载deploy.yaml
https://github.com/kubernetes/ingress-nginx/blob/main/deploy/static/provider/baremetal/deploy.yaml
## 替换镜像url
```
将
k8s.gcr.io/ingress-nginx/controller:v1.1.0@sha256:f766669fdcf3dc26347ed273a55e754b427eb4411ee075a53f30718b4499076a
替换为
registry.cn-hangzhou.aliyuncs.com/cuiw/k8s.gcr.io-ingress-nginx-controller:v1.1.0


将
k8s.gcr.io/ingress-nginx/kube-webhook-certgen:v1.1.1@sha256:64d8c73dca984af206adf9d6d7e46aa550362b1d7a01f3a0a91b20cc67868660
替换为
registry.cn-hangzhou.aliyuncs.com/cuiw/k8s.gcr.io_ingress-nginx_kube-webhook-certgen:v1.1.1
```

# 安装
```
kubectl apply -f deploy.yaml
```