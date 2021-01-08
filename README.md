# SQL IaaS Agent Extension for Microsoft Azure Government 

This repository is to help provide guidance and scripts on how to bulk register SQL Server Virtual Machines in Azure with the Azure SQL IaaS Agent Extension in Azure Government. To see how to review you can view my [video](https://www.youtube.com/watch?v=qmB3ufHN9Kk) on running scripts to register your SQL VMs.

The .psm1 script in this repository is the same one used in the video, but comes pre modified:
```
- [x] Modified to work from Azure Cloud Shell
- [x] Modified to log into Azure Government
```
### High Level List of Capabilities Enabled by SQL IaaS Agent Extension
Capability | Lightweight mode | Full Mode
------------ | ------------- | ------------
HA/Distaster Recovery License Type<br><sub>Take advantage of HA/DR</sub> | :heavy_check_mark: | :heavy_check_mark:
Flexible Licensing<br><sub>Switch Between PAYGO and AHB</sub> | :heavy_check_mark: | :heavy_check_mark:
Unified Management View<br><sub>Managed your SQL VM/PaaS Deloyments from one location</sub> | :heavy_check_mark: | :heavy_check_mark:
Automated Backup<br><sub>Easy backup with Point-in-Time Restore</sub> | :x: | :heavy_check_mark:
Automated Patching<br><sub>Free, Simple installation of Critical Updates (2008 R2+)</sub> | :x: | :heavy_check_mark:
Disk Scaling<br><sub>Resize Data and Log disks from the Azure Portal</sub> | :x: | :heavy_check_mark:
Simplified Always On HA<br><sub>Create Availability Groups with Azure CLI (GUI in Preview as of Oct 2020)</sub> | :x: | :heavy_check_mark:
Azure Key Vault Ingegration<br><sub>Configure Azure Key Vault for the SQL Server instance</sub> | :x: | :heavy_check_mark:
Add'l Integration with Azure<br><sub>Tighter integration with Azure Defender, Vulnerability Assessment and<br>Monitoring services</sub> | CY21 | CY21

### Coming soon to Azure Government

Many of your will know that there is now an "Easy Button" that will help you conduct [auto-registration](https://docs.microsoft.com/en-us/azure/azure-sql/virtual-machines/windows/sql-agent-extension-automatic-registration-all-vms?tabs=azure-cli) of SQL Virtual Machines currently in Azure Commerical regions. While the capability doesn't exist in Azure Government today (Early Jan 2021), the engineering teams are working to enable the feature across Azure Government as well. Once that feature is available, expect this documentation to be updated.
