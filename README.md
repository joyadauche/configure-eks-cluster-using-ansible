# Goal
Install and Configure tools like prometheus, grafana, alertmanager, argocd on an EKS cluster

# Pre-requisites
- [Install python3 and pip3 on the Control Node](https://www.python.org/downloads/)
- [Install ansible on the Control Node](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#control-node-requirements)
- Ensure Python3 is avaialbe on the Managed Nodes by running `python3 --version`, else install it
- Install all package requirements for the ansible modules used. For example, for [kubernetes.core.k8s](https://docs.ansible.com/ansible/latest/collections/kubernetes/core/k8s_module.html#requirements), install the **kubernetes** python package by running, `pip3 install kubernetes`

# Run
`ansible-playbook prometheus-grafana-alertmanager-argocd.yaml`