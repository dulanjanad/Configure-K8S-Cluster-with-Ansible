# Configure-K8S-Cluster-with-Ansible
 Configure Kubernetes Cluster with Ansible

### Prerequisites

* One or more machines running a deb/rpm-compatible Linux OS; for example: Ubuntu or CentOS.
* 2 GiB or more of RAM per machine
* At least 2 CPUs on the machine that you use as a control-plane node.
* Full network connectivity among all machines in the cluster. You can use either a public or a private network.
* A Linux user with permission to login to all of the machines with ssh and ability for privillage escaltion

You can fulfill above mentioned using below repository
https://github.com/dulanjanad/AWS-Playground

### Steps to follow

1). Change ansible.cfg file and inventory file accordingly

2). Run playbooks as below
       
       ansible-playbook set-kubernetes-env.yml
       ansible-playbook initialize-kubernetes-cluster.yml
       ansible-playbook join-workers.yml
