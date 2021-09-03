# 本地镜像


```
# dashboard
docker pull kubernetesui/dashboard:v2.3.1
docker tag kubernetesui/dashboard:v2.3.1 registry.cw.net:5000/kubernetesui/dashboard:v2.3.1
docker rmi kubernetesui/dashboard:v2.3.1
docker push registry.cw.net:5000/kubernetesui/dashboard:v2.3.1

docker pull kubernetesui/metrics-scraper:v1.0.6
docker tag kubernetesui/metrics-scraper:v1.0.6 registry.cw.net:5000/kubernetesui/metrics-scraper:v1.0.6
docker rmi kubernetesui/metrics-scraper:v1.0.6
docker push registry.cw.net:5000/kubernetesui/metrics-scraper:v1.0.6

# flannel
docker pull quay.io/coreos/flannel:v0.14.0
docker tag quay.io/coreos/flannel:v0.14.0 registry.cw.net:5000/quay.io/coreos/flannel:v0.14.0
docker rmi quay.io/coreos/flannel:v0.14.0
docker push registry.cw.net:5000/quay.io/coreos/flannel:v0.14.0


# ingress-nginx
docker pull k8s.gcr.io/ingress-nginx/controller:v1.0.0@sha256:0851b34f69f69352bf168e6ccf30e1e20714a264ab1ecd1933e4d8c0fc3215c6
docker tag k8s.gcr.io/ingress-nginx/controller:v1.0.0@sha256:0851b34f69f69352bf168e6ccf30e1e20714a264ab1ecd1933e4d8c0fc3215c6 registry.cw.net:5000/k8s.gcr.io/ingress-nginx/controller:v1.0.0
docker rmi k8s.gcr.io/ingress-nginx/controller:v1.0.0@sha256:0851b34f69f69352bf168e6ccf30e1e20714a264ab1ecd1933e4d8c0fc3215c6
docker push registry.cw.net:5000/k8s.gcr.io/ingress-nginx/controller:v1.0.0

docker pull k8s.gcr.io/ingress-nginx/kube-webhook-certgen:v1.0@sha256:f3b6b39a6062328c095337b4cadcefd1612348fdd5190b1dcbcb9b9e90bd8068
docker tag k8s.gcr.io/ingress-nginx/kube-webhook-certgen:v1.0@sha256:f3b6b39a6062328c095337b4cadcefd1612348fdd5190b1dcbcb9b9e90bd8068 registry.cw.net:5000/k8s.gcr.io/ingress-nginx/kube-webhook-certgen:v1.0
docker rmi k8s.gcr.io/ingress-nginx/kube-webhook-certgen:v1.0@sha256:f3b6b39a6062328c095337b4cadcefd1612348fdd5190b1dcbcb9b9e90bd8068
docker push registry.cw.net:5000/k8s.gcr.io/ingress-nginx/kube-webhook-certgen:v1.0
```