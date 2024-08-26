```
kube-apiserver -h | grep enable-admission-plugins
```

If you are running in kubeadm based setup

```
kubectl exec kube-apiserver-controlplane -n kube-system -- kube-apiserver -h | grep enable-admission-plugins
```
