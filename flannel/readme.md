# 准备
## 下载kube-flannel.yml
https://github.com/flannel-io/flannel/blob/master/Documentation/kube-flannel.yml
## 修改kube-flannel.yml，指定eth1
```
...

      containers:
      - name: kube-flannel
        image: 192.168.10.104:5000/quay.io/coreos/flannel:v0.14.0
        command:
        - /opt/bin/flanneld
        args:
        - --ip-masq
        - --kube-subnet-mgr
        - --iface=eth1

...
```

# 安装
```
kubectl apply -f kube-flannel.yml
```