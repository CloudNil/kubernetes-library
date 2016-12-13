# kubernetes-library
#### kubernetes v1.5.0 dependency:
- etcd-amd64:2.2.5
- kubedns-amd64:1.7
- kube-dnsmasq-amd64:1.3 
- exechealthz-amd64:1.1 
- pause-amd64:3.0
- kube-discovery-amd64:1.0
- kube-proxy-amd64:v1.5.0 
- kube-scheduler-amd64:v1.5.0
- kube-controller-manager-amd64:v1.5.0 
- kube-apiserver-amd64:v1.5.0 
- kubernetes-dashboard-amd64:v1.5.0

#### usage:
```bash
#!/bin/bash
images=(kube-proxy-amd64:v1.5.0 kube-discovery-amd64:1.0 kubedns-amd64:1.7 kube-scheduler-amd64:v1.5.0 kube-controller-manager-amd64:v1.5.0 kube-apiserver-amd64:v1.5.0 etcd-amd64:2.2.5 kube-dnsmasq-amd64:1.3 exechealthz-amd64:1.1 pause-amd64:3.0 kubernetes-dashboard-amd64:v1.5.0)
for imageName in ${images[@]} ; do
  docker pull cloudnil/$imageName
  docker tag cloudnil/$imageName gcr.io/google_containers/$imageName
  docker rmi cloudnil/$imageName
done
```