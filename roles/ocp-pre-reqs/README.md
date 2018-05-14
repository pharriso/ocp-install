Role Name
=========

This role configures the OCP pre-reqs as per the Red Hat OCP host prepartion section:

https://access.redhat.com/documentation/en-us/openshift_container_platform/3.9/html/installation_and_configuration/installing-a-cluster#install-config-install-host-preparation

Requirements
------------

SSH keys need to be generated and copied to all of the nodes that OCP will be installed on.

Role Variables
--------------

docker_disk_name: The name of the disk that will be used for docker storage. Default is vdb
rhsm_register: Whether to register to RHSM
rhsm_user: User to register to RHSM
rhsm_pass: Password to register to RHSM
rhsm_pool: Pool ID which contains OCP subs
