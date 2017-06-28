# kubernetes-library

#### kubernetes v1.6.6 dependency:
- etcd-amd64:3.0.17
- pause-amd64:3.0
- kube-proxy-amd64:v1.6.6 
- kube-scheduler-amd64:v1.6.6
- kube-controller-manager-amd64:v1.6.6 
- kube-apiserver-amd64:v1.6.6
- kubernetes-dashboard-amd64:v1.6.1
- k8s-dns-sidecar-amd64:1.14.2
- k8s-dns-kube-dns-amd64:1.14.2
- k8s-dns-dnsmasq-nanny-amd64:1.14.2

```bash
#!/bin/bash
images=(kube-proxy-amd64:v1.6.6 kube-scheduler-amd64:v1.6.6 kube-controller-manager-amd64:v1.6.6 kube-apiserver-amd64:v1.6.6 etcd-amd64:3.0.17 pause-amd64:3.0 kubernetes-dashboard-amd64:v1.6.1 k8s-dns-sidecar-amd64:1.14.2 k8s-dns-kube-dns-amd64:1.14.2 k8s-dns-dnsmasq-nanny-amd64:1.14.2)
for imageName in ${images[@]} ; do
  docker pull cloudnil/$imageName
  docker tag cloudnil/$imageName hub.lonhwin.com/$imageName
  docker push hub.lonhwin.com/$imageName
  #docker tag cloudnil/$imageName gcr.io/google_containers/$imageName
  docker rmi cloudnil/$imageName
done
```
