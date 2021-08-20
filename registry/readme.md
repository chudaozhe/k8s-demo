# 本地镜像


```
docker pull quay.io/coreos/flannel:v0.14.0
docker tag quay.io/coreos/flannel:v0.14.0 192.168.10.104:5000/quay.io/coreos/flannel:v0.14.0
docker rmi quay.io/coreos/flannel:v0.14.0


docker pull k8s.gcr.io/ingress-nginx/controller:v0.48.1@sha256:e9fb216ace49dfa4a5983b183067e97496e7a8b307d2093f4278cd550c303899
docker tag k8s.gcr.io/ingress-nginx/controller:v0.48.1 192.168.10.104:5000/k8s.gcr.io/ingress-nginx/controller:v0.48.1
docker rmi k8s.gcr.io/ingress-nginx/controller:v0.48.1

docker pull docker.io/jettech/kube-webhook-certgen:v1.5.1
docker tag docker.io/jettech/kube-webhook-certgen:v1.5.1 192.168.10.104:5000/docker.io/jettech/kube-webhook-certgen:v1.5.1
docker rmi docker.io/jettech/kube-webhook-certgen:v1.5.1
```