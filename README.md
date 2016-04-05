# Ansible Module : Vagrant

##Install
In the *library* subdirectory is the `vagrant.py` module file.  The easiest way to make use of this module at this point is to create a `/library` subdirectory in your Ansible playbook project and copy the file there.  Ansible will search this directory by default for modules.

##Actions
- init
  - This will create a vagrant file according to the profile specified in the playbook task.
- up
  - This will attempt to start up a system based on an existing vagrant file.
- init-up
  - This action combines both the *init* and *up* into a single action. 
- halt
  - This action will attempt to stop a running vagrant system.
- destroy
  - This action will remove a vagrant system.

##Examples
Please see the example playbook files in this project for examples on how to use all the actions.

## Dependencies
This module is designed to work with Ansible 1.9 and 2.x.

This module expects to find *Vagrant* and *virtualbox* (vboxmanage) commands and utilities in the default path.

Please refer to the specific practices for your platform regarding the installation of *Vagrant* and *virtualbox*
