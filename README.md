# Kubeadm-CalicoCloud
Install Kubernetes (with Docker by default) + Calico Cloud (ESXi/Ubuntu/OnPrem)

In this exercise we need 3 Linux nodes freshly installed, updated and that are on the same network.
They can be located on any hypervisors (Hyper-V, ESXi, VirtualBox etc.).

I have chosen to use 3 Ubuntu servers on my VMware vSphere Cluster of 2 ESXi Hosts.
The hosts and VMs are on the same network as the lan to make it easier to manage them.

The Virtual Machines are called Kube1, Kube2 and Kube3 with the IP 192.168.0.37, 192.168.0.38, 192.168.0.39.

The steps are:
Linux: Install, update, snapshot
Docker: Basic install
Kubernetes: Install the Master node, join the 2 others.
Calico Cloud

## Sources and Pre-requierements

Install and Configure ESXi Host
```
https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.esxi.install.doc/GUID-93D0227B-E5ED-40B0-B8E2-71141A32EB00.html
```
Deploy a Virtual Machine
```
https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.vsphere.vm_admin.doc/GUID-AE8AFBF1-75D1-4172-988C-378C35C9FAF2.html?hWord=N4IghgNiBcIG4EsBOAXArpABAWzAYwAsEA7AUxAF8g
```
Install Ubuntu Server
```
https://ubuntu.com/tutorials/install-ubuntu-server#1-overview
```
Install Docker for Ubuntu
```
https://docs.docker.com/engine/install/ubuntu/
```
Install Kubernetes on Linux
```
https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/install-kubeadm/
```
Install Project Calico
```
https://projectcalico.docs.tigera.io/getting-started/kubernetes/self-managed-onprem/onpremises
```
Install and Configure Calicoctl
```
https://projectcalico.docs.tigera.io/maintenance/clis/calicoctl/install
```
Connect your Kubernetes cluster to Calico Cloud
```
https://tigera.awsworkshop.io/040_calico_setup/joinekstocalicocloud.html
```
