# 准备
## 下载deploy.yaml
https://github.com/kubernetes/ingress-nginx/blob/main/deploy/static/provider/baremetal/deploy.yaml
## 替换镜像url
```
#192.168.10.104:5000为本地镜像
将
k8s.gcr.io/ingress-nginx/controller:v0.48.1@sha256:e9fb216ace49dfa4a5983b183067e97496e7a8b307d2093f4278cd550c303899
替换为
192.168.10.104:5000/k8s.gcr.io/ingress-nginx/controller:v0.48.1


将
docker.io/jettech/kube-webhook-certgen:v1.5.1
替换为
192.168.10.104:5000/docker.io/jettech/kube-webhook-certgen:v1.5.1
```

# 安装
```
kubectl apply -f deploy.yaml

kubectl apply -f nginx-deployment.yaml
kubectl apply -f nginx-service.yaml

kubectl apply -f test-ingress.yml
```