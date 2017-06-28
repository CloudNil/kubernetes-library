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

```bash
#!/bin/bash
images=(kube-proxy-amd64:v1.5.0 kube-discovery-amd64:1.0 kubedns-amd64:1.7 kube-scheduler-amd64:v1.5.0 kube-controller-manager-amd64:v1.5.0 kube-apiserver-amd64:v1.5.0 etcd-amd64:2.2.5 kube-dnsmasq-amd64:1.3 exechealthz-amd64:1.1 pause-amd64:3.0 kubernetes-dashboard-amd64:v1.5.0)
for imageName in ${images[@]} ; do
  docker pull cloudnil/$imageName
  docker tag cloudnil/$imageName gcr.io/google_containers/$imageName
  docker rmi cloudnil/$imageName
done
```



#### kubernetes v1.5.1 dependency:
- etcd-amd64:2.2.5
- kubedns-amd64:1.7
- kube-dnsmasq-amd64:1.3 
- exechealthz-amd64:1.1 
- pause-amd64:3.0
- kube-discovery-amd64:1.0
- kube-proxy-amd64:v1.5.1 
- kube-scheduler-amd64:v1.5.1
- kube-controller-manager-amd64:v1.5.1 
- kube-apiserver-amd64:v1.5.1 
- kubernetes-dashboard-amd64:v1.5.0

```bash
#!/bin/bash
images=(kube-proxy-amd64:v1.5.1 kube-discovery-amd64:1.0 kubedns-amd64:1.7 kube-scheduler-amd64:v1.5.1 kube-controller-manager-amd64:v1.5.1 kube-apiserver-amd64:v1.5.1 etcd-amd64:2.2.5 kube-dnsmasq-amd64:1.3 exechealthz-amd64:1.1 pause-amd64:3.0 kubernetes-dashboard-amd64:v1.5.0)
for imageName in ${images[@]} ; do
  docker pull cloudnil/$imageName
  docker tag cloudnil/$imageName gcr.io/google_containers/$imageName
  docker rmi cloudnil/$imageName
done
```



#### kubernetes v1.5.2 dependency:
- etcd-amd64:2.2.5
- kubedns-amd64:1.9
- kube-dnsmasq-amd64:1.4 
- dnsmasq-metrics-amd64:1.0
- exechealthz-amd64:1.2 
- pause-amd64:3.0
- kube-discovery-amd64:1.0
- kube-proxy-amd64:v1.5.2 
- kube-scheduler-amd64:v1.5.2
- kube-controller-manager-amd64:v1.5.2 
- kube-apiserver-amd64:v1.5.2 
- kubernetes-dashboard-amd64:v1.5.0

```bash
#!/bin/bash
images=(kube-proxy-amd64:v1.5.2 kube-discovery-amd64:1.0 kubedns-amd64:1.9 kube-scheduler-amd64:v1.5.2 kube-controller-manager-amd64:v1.5.2 kube-apiserver-amd64:v1.5.2 etcd-amd64:2.2.5 kube-dnsmasq-amd64:1.4 dnsmasq-metrics-amd64:1.0 exechealthz-amd64:1.2 pause-amd64:3.0 kubernetes-dashboard-amd64:v1.5.0)
for imageName in ${images[@]} ; do
  docker pull cloudnil/$imageName
  docker tag cloudnil/$imageName gcr.io/google_containers/$imageName
  docker rmi cloudnil/$imageName
done
```


#### kubernetes v1.6.6 dependency:
- etcd-amd64:3.0.17
- pause-amd64:3.0
- kube-proxy-amd64:v1.6.6 
- kube-scheduler-amd64:v1.6.6
- kube-controller-manager-amd64:v1.6.6 
- kube-apiserver-amd64:v1.6.6
- kubernetes-dashboard-amd64:v1.6.1
- k8s-dns-sidecar-amd64:1.14.1
- k8s-dns-kube-dns-amd64:1.14.1
- k8s-dns-dnsmasq-nanny-amd64:1.14.1

```bash
#!/bin/bash
images=(kube-proxy-amd64:v1.6.6 kube-scheduler-amd64:v1.6.6 kube-controller-manager-amd64:v1.6.6 kube-apiserver-amd64:v1.6.6 etcd-amd64:3.0.17  pause-amd64:3.0 kubernetes-dashboard-amd64:v1.6.1 k8s-dns-sidecar-amd64:1.14.1 k8s-dns-kube-dns-amd64:1.14.1 k8s-dns-dnsmasq-nanny-amd64:1.14.1)
for imageName in ${images[@]} ; do
  docker pull cloudnil/$imageName
  docker tag cloudnil/$imageName gcr.io/google_containers/$imageName
  docker rmi cloudnil/$imageName
done
```