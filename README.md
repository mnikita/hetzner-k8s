
#### Automated Kubernetes deployment on Hetzner Cloud

##### Summary:
Kubernetes cluster deployment on Hetzner infrastructure using a Kubernetes management platform. Automated, extendable deployment with updates, backups and restores. The deployment procedure is reproducible for virtual Hetzner cloud instances and dedicated servers. 

##### Description:
Creation of automated procedure for provisioning cloud instances and dedicated servers on Hetzner Cloud infrastructure. Preferred deployment tool is Terraform. Ideally, the whole deployment procedure is driven by a simple YAML config file. Suggestions for a different Kubernetes management platform / tools are welcome.

The following features are required for the deployment.

##### Features:
- Provisioning of Hetzner cloud instances / dedicated servers 
- Provisioning of Hetzner hardware Load Balancer
- Block Storage
- Dynamic PV provisioner for block storage
- FS Storage
- Dynamic PV provisioner for FS storage
- Snapshot / Backup / Restore using Velero to a dedicated Hetzner storage box
- Cluster upgrade procedure
- Monitoring + Alerting
- Volume Replication

##### Validation:
- Deployed Kubernetes Pod with FS volume mounted and simple read/write operation
- Deployed Kubernetes Pod with block device mounted and simple read/write operation
- Deployed Kubernetes Service for pods with type Load Balancer
- Validation of monitoring / alerting dashboard

