Role Name
=========

These roles prepare a bastion or install host to deploy OCP. It also runs the necessary pre-reqs for deploying OCP. These can be used to deliver OCP PoC's.

Installation
------------

* Populate the hosts file with the list of OCP hosts.
* Register the bastion to RHSM or Satellite.
* Enable the relevant repos.
	- rhel-7-server-rpms
	- rhel-7-server-extras-rpms
	- rhel-7-server-ose-3.9-rpms 
	- rhel-7-server-ansible-2.4-rpms
* Generate a SSH keypair on the bastion.
* Copy the public key to all OCP hosts.
* Edit variables to suit your environment.
* Run the playbooks. e.g.
		ansible-playbook -i hosts ocp-pre-reqs.yml
