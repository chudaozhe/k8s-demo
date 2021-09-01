# 准备
## 下载deploy.yaml
https://github.com/kubernetes/ingress-nginx/blob/main/deploy/static/provider/baremetal/deploy.yaml
## 替换镜像url
```
#192.168.10.104:5000为本地镜像
将
k8s.gcr.io/ingress-nginx/controller:v1.0.0@sha256:0851b34f69f69352bf168e6ccf30e1e20714a264ab1ecd1933e4d8c0fc3215c6
替换为
192.168.10.104:5000/k8s.gcr.io/ingress-nginx/controller:v1.0.0


将
k8s.gcr.io/ingress-nginx/kube-webhook-certgen:v1.0@sha256:f3b6b39a6062328c095337b4cadcefd1612348fdd5190b1dcbcb9b9e90bd8068
替换为
192.168.10.104:5000/k8s.gcr.io/ingress-nginx/kube-webhook-certgen:v1.0
```

# 安装
```
kubectl apply -f deploy.yaml

kubectl apply -f nginx-deployment.yaml
kubectl apply -f nginx-service.yaml

kubectl apply -f test-ingress.yml
```