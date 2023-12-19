# Kubian
Connecting all sorts of computers into a [Kubernetes](https://kubernetes.io) (version 1.28) cluster based on [Debian 12](https://www.debian.org)

## Feature list

* simple setup procedure using `kubeadm`
    - CNI: [flanell](https://github.com/flannel-io/flannel)
    - cgroups
* one master node
* compute nodes run in virtual machines with a bridged network interface
    - Windows: [VirtualBox](https://www.virtualbox.org/)
    - macOS: [UTM](https://mac.getutm.app/)
    - Linux: [libvirtd](https://libvirt.org/)
    - FreeBSD: [bhyve](https://docs.freebsd.org/en/books/handbook/virtualization/#virtualization-bhyve-zfs)
* node metrics captured with [Prometheus](https://prometheus.io) and visualised using [Grafana](https://grafana.com)
    - project: [kube-prometheus](https://github.com/prometheus-operator/kube-prometheus)
* management console [OpenLens](https://github.com/MuhammedKalkan/OpenLens)
* private Docker image registry to feed your pods
    - image: [registry:2](https://hub.docker.com/_/registry)


## Wish list

* upgrade Kubernetes to new version
* more master nodes for redundancy
* joining of mobile phones running "termux" or "userland" (?)
* joining of 32bit armv7 SBC boards (?)
* job queueing system
