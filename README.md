# kubernetes-library

#### kubernetes v1.11.0 dependency:
- etcd-amd64:3.2.18
- pause-amd64:3.1
- kube-proxy-amd64:v1.11.0 
- kube-scheduler-amd64:v1.11.0
- kube-controller-manager-amd64:v1.11.0 
- kube-apiserver-amd64:v1.11.0
- k8s.gcr.io/coredns:1.1.3

```bash
#!/bin/bash
images=(kube-proxy-amd64:v1.11.0 kube-scheduler-amd64:v1.11.0 kube-controller-manager-amd64:v1.11.0 kube-apiserver-amd64:v1.11.0 etcd-amd64:3.2.18 pause-amd64:3.1)
for imageName in ${images[@]} ; do
  docker pull cloudnil/$imageName
done
```
