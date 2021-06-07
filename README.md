cloud-inventory
========

#### OpenStack Infrastructure Inventory ####

This module provides an abstraction layer to inventory your cloud resources.

Supported services (and APIs):
`EC2:`

Supported Regions
`us-west-1`

### Installation ###
```bash
npm install openstack-inventory
```

### Usage ###

```javascript
import OpenstackInventory from 'openstack-inventory'

const config = {
  credentials: {
    accessKeyId: 'your_access_key',
    secretAccessKey: 'your_secret_key'
  },
  services: ['ec2', 'rds'],
  regions: ['us-west-2, us-east-1']
};

const oInventory = new OpenstackInventory(config);
const oResources = oInventory.inventory();
```
