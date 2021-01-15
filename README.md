# k8s-simple-node

kubeadm init --apiserver-advertise-address $(hostname -i) --pod-network-cidr 10.5.0.0/16

kubectl apply -f https://raw.githubusercontent.com/cloudnativelabs/kube-router/master/daemonset/kubeadm-kuberouter.yaml

kubectl apply -f https://raw.githubusercontent.com/kubernetes/website/master/content/en/examples/application/nginx-app.yaml

kubectl apply -f https://cloud.weave.works/k8s/net" 

kubeadm join 192.168.0.13:6443 --token 0xufls.x0p1nuibztmq4i1i \
    --discovery-token-ca-cert-hash sha256:57e144083633326b1fcfe40b2506598b38523103b27193fad67a7d9fe21dee06

kubectl get nodes
