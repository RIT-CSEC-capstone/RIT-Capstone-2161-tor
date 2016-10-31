# Openstack Tor Project

## Versions
- Python 3.5.2
- Pip 8.1.2

## Dependencies
- python-openstackclient

## Imports
- import time
- import getpass
- from novaclient.client import Client

## Functions
### Reporting
- list_servers
  * Lists running instances
- list_images
  * Lists available images
- list_flavors
  * Lists available flavors
- list_networks
  * Lists available networks

### Instances
- create_instance
  * Creates a new instance based on given name, image, flavor
- terminate_instance 
  * Terminates an instance based on given name
  
## TODO
- Fix rename_instance
- Add JSON input support
- Make instance creation more configurable
- Add support for updating instances post-creation
- Add userdata field in create_instance to pass post-creation scripts
  
## Reference
- http://docs.openstack.org/developer/python-novaclient/ref/v2/client.html
- http://docs.openstack.org/user-guide/sdk-compute-apis.html#create-server-api-v2