All right: 

got 5 VMS in AWS : using kubeadm we are setting up the cluster

KUBE_HA_PROXY : 172.31.29.162
KUBE_HA_CONTROL1: 172.31.20.245  
KUBE_HA_CONTROL2: 172.31.26.232
KUBE_HA_COMPUTE1: 172.31.17.57
KUBE_HA_COMPUTE2: 172.31.28.158

plan: 
2 control plane vms - via 1 HA proxy LB 
2 compute nodes - 

what all to be installed ? 

Kubectl on all the 5 VM's
conatiner d, (refer docker instalation doc) - on all 4 vms's
kubelet kubeadm kubectl - on all 4 vms 
calico network for kubernetes CNI ( on 4 VM's) IP range used 10.244.0.0/16
