### Required packages:

* Vagrant
* Virtualbox
* Ansible

### How to use:

1. Clone this repository:


2. Go up the virtual machines: 
```
$ vagrant up wordpress && vagrant up mysql
```
3. Execute Ansible script:

*It is important to check if the Vagrant key path is correct*
```
$ ansible-playbook provisioning.yml -i hosts
```

#### Note:
You can also use the Ansible script without Vagrant with your preferred host. To do this, change the data of the `hosts` and `group_vars` file.
