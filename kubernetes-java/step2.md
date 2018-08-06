Initialize the cluster with the Token
`kubeadm init --token=102952.1a7dd4cc8d1f4cc5 --kubernetes-version $(kubeadm version -o short)`{{execute}}

`sudo cp /etc/kubernetes/admin.conf $HOME/`{{execute}} 
`sudo chown $(id -u):$(id -g) $HOME/admin.conf`{{execute}} 
`export KUBECONFIG=$HOME/admin.conf
`{{execute}}

Copy the join command and execute on the Node host
