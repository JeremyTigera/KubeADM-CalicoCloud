# KubeADM-CalicoCloud
Install Docker + Kubernetes + Calico Cloud (ESXi/Ubuntu/OnPrem)

In this exercise we need 3 Linux nodes freshly installed, updated that are on the same network.
They can be located on any hypervisor (Hyper-V, ESXi, VirtualBox etc.).

I have chosen to use 3 Ubuntu servers on my VMware vSphere Cluster of 2 ESXi Hosts.
The hosts and VMs are on the same network as the lan to make it easier to manage them.

VMs are called Kube1, Kube2 and Kube3 with the IP 192.168.0.37, 192.168.0.38, 192.168.0.39.

The steps are:
Linux: Install, update, snapshot
Docker: Basic install
Kubernetes: Install the Master node, join the 2 others.
Calico Cloud
