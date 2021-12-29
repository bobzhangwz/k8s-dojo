
# Prerequisite

Run commands list below: 
```
ansible-galaxy install -r requirements.yml
```

# How



## Run kubectl in local
```
export KUBECONFIG=$KUBECONFIG:$HOME/.kube/vagrant_conf
kubectl get pods -n kube-system
```
