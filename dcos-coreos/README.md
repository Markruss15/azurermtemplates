# Deploy a Mesosphere Datacenter Operating System (DCOS) cluster on Azure

<a href="https://azuredeploy.net/" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

This template deploys a DCOS cluster on Azure.

Below are the parameters that the template expects

| Name   | Description    |
|:--- |:---|
| adminUsername | Admin username used when provisioning virtual machines |
|storageAccountName | Unique namespace for the Storage Account where the Virtual Machine's disks will be placed |
| region | Location where resources will be provisioned |
| virtualNetworkName | Virtual Network |
| vmSizeMasterNodes | Size of the Master nodes |
| vmSizeSlaveNodes | Size of the Slave nodes |
| numberOfMasters | Number of Master nodes (1, 3, or 5) |
| numberOfSlaves | Number of Slave nodes |
| addressPrefix | Address space for the VNET |
| subnet1Name | Subnet name for the VNET that resources will be provisionined in to |
| subnet1Prefix | Address space for the subnet | 
| sshKeyData | Public key for SSH authentication |
| uuid | Globally unique cluster identifier in Azure namespace |
| azureAccountName | Azure account name used by Exhibitor to persist Zookeeper state |
| azureAccountKey | Azure account key used by Exhibitor to persist Zookeeper state |