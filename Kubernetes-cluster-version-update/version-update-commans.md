## Master node upgrades

    1  sudo -i
    2  kubectl get nodes
    3  kubectl version
    4  kubectl version short
    5  kubectl version
    6  kubectl version --short
### Unholding the kubeadm
    7  sudo apt-mark unhold kubeadm
### updating the kubeadm with specific versions
    8  sudo apt install -y kubeadm=1.16.6-00
    9  sudo kubeadm upgrade plan
### Components that must be upgraded manually after you have upgraded the control plane with 'kubeadm upgrade apply'
![image]https://github.com/chaets/Kubernetes-essentials/blob/master/Kubernetes-cluster-version-update/adm-components.JPG
    10  sudo kubeadm upgrade apply v1.16.6
### unholding the kubelet
    11  sudo apt-mark unhold kubelet
### updating the kubelet with specific versions
    12  sudo apt install -y kubelet=1.16.6-00
### Unholding the kubectl
    13  sudo apt-mark unhold kubectl
### updating the kubectl with specific versions
    14  sudo apt install -y kubectl=1.16.6-00
    15  kubectl version --short


## Worker Node updates
As there be only kubelet running at the worker nodes, so only kubelet needs to update

### updating the kubelet with specific versions
    12  sudo apt install -y kubelet=1.16.6-00
### Unholding the kubectl
    13  sudo apt-mark unhold kubectl
