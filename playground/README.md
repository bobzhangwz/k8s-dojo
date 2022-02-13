
# Prerequisite(Not follow)

Run commands list below: 
```
ansible-galaxy install -r requirements.yml
```

# How

```
vagrant up m1 s1 
# vagrant destroy
# vagrant halt
# vagrant ssh m1
# vagrant ssh s1
ansible-playbook -i dev main.yml
```


## Reources

* https://kubernetes.io/docs/tasks/debug-application-cluster/debug-service/
* https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/troubleshooting-kubeadm/
* https://computingforgeeks.com/deploy-kubernetes-cluster-on-ubuntu-with-kubeadm/
* https://www.digitalocean.com/community/tutorials/how-to-create-a-kubernetes-cluster-using-kubeadm-on-ubuntu-20-04


## Run kubectl in local

```
export KUBECONFIG=$KUBECONFIG:$HOME/.kube/vagrant_conf
kubectl get pods -n kube-system

# scheduled to master node
kubectl taint nodes --all node-role.kubernetes.io/master-
```
