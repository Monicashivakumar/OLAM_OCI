# Oracle Linux Automation Manager on OCI

## Introduction
Oracle Linux Automation Manager is an automation tool for deploying software, configuring systems, and orchestrating tasks such as upgrades and updates, in the form of playbooks.
Based on the open source project AWX, this tool provides a Web interface for scheduling and running playbook tasks on the inventories the playbooks interact with. 
The Oracle Cloud Infrastructure (OCI) Ansible Collection provides an easy way to provision and manage resources in the Oracle Cloud using Ansible. The same collections can be leveraged from Oracle Linux Automation Manager to automate and manage Oracle Cloud Infrasturcutre

## Using OCI Ansible Collections

To leverage OCI Ansible collections in Oracle Linux Automation Manager in order to automate and manage OCI Environments, there are two ways:

* Including OCI Collections in SCM Based Projects: Detailed steps on using OCI Ansible collections is documented [here](https://docs.oracle.com/en/learn/olam-oci-collection/#create-a-playbook).
* Customizing Execution Environments: Starting Oracle Linux Automation Manager v2.1, there is feature added to customize the execution environments to include required collections, OCI Anisble collections for example. 

## OCI Dynamic Inventories 

Oracle Linux Automation Manager uses inventory  to work against managed nodes or hosts in your infrastructure. This inventory contains a list of servers, their IP addresses, and other optional connection information.
A static inventory file works well if your infrastructure hardly changes.
However, your infrastructure is likely in constant flux when using the cloud. Therefore it would be great to have a way to have your inventory dynamically updated as hosts come and go.

Here are the steps 

To use OCI Dyanmic Inventories with Oracle Linux Automation Manager, follow the detailed instructions at:
https://docs.oracle.com/en/learn/olae-dyninv/#setup-oracle-cloud-infrastructure-sdk-for-python
