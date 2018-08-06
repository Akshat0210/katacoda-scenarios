For similicity let deploy weave network. There are multiple option for network plug-in please check K8 documentation.

`kubectl apply -f /opt/weave-kube`{{execute}}

Verify Pods are running.  `kubectl get pod -n kube-system`{{execute}}

Once all pods are running check if the node is ready to deploy the container. 
`kubectl get nodes`{{execute}}

Deploy the sample container.
`kubectl run http --image=katacoda/docker-http-server:latest --replicas=1`{{execute}}

Verify pods are running 
`kubectl get pods`{{execute}}
