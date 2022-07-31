## Run eksctl to create the EKS cluster using the config yaml file

**Create cluster and update .kube config file**

```
$ eksctl create cluster -f eks_config.yaml

$ aws eks update-kubeconfig --name clo835 --region us-east-1
```

**Confirm EKS cluster is running and worker nodes in “Ready” state**

```
$ k get nodes

$ k cluster-info

$ k get all --all-namespaces
```
