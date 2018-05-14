Role Name
=========

This role prepares a host to run the openshift-ansible playbook to install OpenShift Container Platform

Requirements
------------

SSH keys need to be generated and copied to all of the nodes that OCP will be installed on.

Role Variables
--------------

This role generates the OCP ansible inventory file using a template. The following variables can be modified

deploy_cns: Whether we want to deploy CNS
cns_disk_name: The name of the disk that will used for the CNS gluster disk. Defaults to vdc
ocp_default_domain: Default apps subdomain. E.g. apps.example.com
ocp_cluster_vip_name: Cluster VIP name that will be used for the master API. e.g. openhift.example.com
