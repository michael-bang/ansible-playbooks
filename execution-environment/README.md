# Creating your own Execution Environment for Ansible Automation Platform

If you need specific ansible collections or applications available in your execution environment then you can use ansible-builder to create these custom containers that can be used from Ansible Automation Platform.

This example creates an execution environment where the mssql collection from galaxy is added and Microsoft Powershell is added through a rpm.

In order to create your own execution environment you need the following:

## Ansible-builder
Ansible-builder can be installed from the ansible repository

## Execution-environmet.yml
The default name for the file defining the new execution environment is execution-environment.yml.

The included example defines a couple of things.

> package_manager_path: /usr/bin/microdnf

If you build upon the default execution environments then the package manager is microdnf and you will need to tell ansible
