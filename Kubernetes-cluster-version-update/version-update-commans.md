Master node upgrades

    1  sudo -i
    2  kubectl get nodes
    3  kubectl version
    4  kubectl version short
    5  kubectl version
    6  kubectl version --short
    7  sudo apt-mark unhold kubeadm
    8  sudo apt install -y kubeadm=1.16.6-00
    9  sudo kubeadm upgrade plan
   10  kubeadm upgrade apply v1.16.7
   11  sudo kubeadm upgrade apply v1.16.7
   12  kubeadm upgrade apply v1.16.7
   13  sudo kubeadm upgrade apply v1.16.6
   14  sudo apt-mark unhold kubelet
   15  sudo apt install -y kubelet=1.16.6-00
   16  sudo apt-mark unhold kubectl
   17  sudo apt install -y kubectl=1.16.6-00
   18  kubectl version --short


Worker Node updates
As there be only kubelet running at the worker nodes, so only kubelet needs to update