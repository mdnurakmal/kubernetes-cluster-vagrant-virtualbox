
# Automatically create kubernetes cluster (1 Master and 2 node) using vagrant

# Prerequisite
- Windows 10

# Installation

Download & Install:
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads) (latest version, tested with 6.1.26)
- [Vagrant](https://www.vagrantup.com/downloads.html) (latest version, tested with 2.2.18)

```shell
vagrant plugin install vagrant-hostmanager
```

## Usage

Create VMs from vagrant file

```shell
vagrant up
```

Connect to master node using SSH

```shell
vagrant ssh master
```

Check kubernetes cluster is up and running <br >
kubectl can only be run on master node

```shell
kubectl get nodes
```

Destroy VMs

```shell
vagrant destroy
```


## References
* https://devopscube.com/kubernetes-cluster-vagrant/
* https://github.com/scriptcamp/vagrant-kubeadm-kubernetes
