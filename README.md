This Document Tell The Kubernetes Cluster Installation With Ansible Automation Platform
If you want install the kubernetes cluster, you should follow below steps; NOTE: This code is only valid for systems with a master and a worker node

==============================================================================

You should create ssh key and copy remote machine or machines:
ssh-keygen
ssh-copy-id root@"your_target_master_machine_ip_adress"
ssh-copy-id root@"your_target_worker_machine_ip_adress"
Then after you just run command and you should looks installation:
ansible-playbook install.yml -i inventory.txt
You can go remote machine and control the kubernetes cluster .
kubectl get nodes
===============================================================================

Install Ansible
-----------------------------

#hostnamectl-sethostname maste
Vim /etc/hosts

create hostname in the each node and add to the hosts file vim /etc/hosts

Yum install epel-release
Yum install ansible

Ssh-keygen
cd .ssh/
ll
Ssh-copy-id root@master.example.com
Ssh-copy-id root@node1.example.com
Ssh-copy-id root@node2.example.com

setting up the ansible cfg file

#ansible masters --list-hosts

#ansible all --list-hosts