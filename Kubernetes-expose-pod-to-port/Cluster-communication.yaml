## Cluster communication

    1  sudo -i
    2  kubectl get nodes
### create a pod with nginx image
    3  kubectl run nginx --image=nginx
    4  kubectl get deployments
### exposing the port of pod using NodePort service
    5  kubectl expose deployment nginx --port 80 --type NodePort
    6  kubectl get service
### to view yaml file for any deployment pod which is running
    7  kubectl get pod nginx-7cdbd8cdc9-x2blp -o yaml
### to view yaml file for any servive pod which is running
    8  kubectl get service nginx -o yaml
### creating the busybox yaml
    9  vim busybox.yml
    10  kubectl create -f busybox.yaml
### checing the fully qualified dns name
    11  kubectl exec busybox -- nslookup nginx