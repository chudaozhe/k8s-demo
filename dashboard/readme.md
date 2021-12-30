# 准备
## 下载recommended.yaml
https://github.com/kubernetes/dashboard/blob/master/aio/deploy/recommended.yaml
# 安装
```
kubectl apply -f recommended.yaml
kubectl apply -f dashboard-svc.yaml
kubectl apply -f dashboard-svc-account.yaml
```
# 文档
http://www.cuiwei.net/p/1987004779