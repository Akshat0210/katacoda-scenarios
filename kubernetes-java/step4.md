Kubernetes provides the base dashboard to visualize the cluster. 

Let install K8 Dashboard
`kubectl apply -f dashboard.yaml`{{execute}}

Verify pods
`kubectl get pods -n kube-system`{{execute}}

Once PODs are ready check the dasboard with below URL

https://[[HOST_SUBDOMAIN]]-9090-[[KATACODA_HOST]].environments.katacoda.com/
