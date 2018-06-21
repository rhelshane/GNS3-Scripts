# Install GNS3 Server 
## Requirements
This script is designed to work on Ubuntu 18.04 LTS. It should be run under root (not suitable for a production environment).
## Actions Performed
* Update system packages
* Install GNS3-Server
* Install Docker
* Install Dynamips
* Install uBridge
* Install VPCS
* Configure UFW
* Configure GNS3
## Installation
Change to root user (if necessary) and clone Git repository:
```
sudo su - 
git clone https://github.com/rhelshane/Install-GNS3-Server.git
```
Enter the new directory, change variables (**GNS_USER** and **GNS_PASS** at a minimum), update permissions, and run setup.sh:
```
cd GNS3-Scripts
vi setup.sh
chmod 744 setup.sh
./setup.sh
```
Start the GNS3 Server:
```
gns3server
```
