# Cisco Catalyst SD-WAN Node Definitions

This directory contains the following node definitions:

* `cat-sdwan-validator.yaml` - Cisco Catalyst SD-WAN Validator (formerly vBond) node definition
* `cat-sdwan-vedge.yaml` - Cisco Catalyst SD-WAN vEdge node definition
* `cat-sdwan-manager.yaml` - Cisco Catalyst SD-WAN Manager (formerly vManage) node definition
* `cat-sdwan-controller.yaml` - Cisco Catalyst SD-WAN Controller (formerly vSmart) node definition
* `cat-sdwan-cedge.yaml` - Cisco Catalyst SD-WAN cEdge node definition

### Image Availability

Images for all nodes except the cat-sdwan-cedge can be downloaded from
https://software.cisco.com/download/home/286320995/type with a proper Cisco.com account and entitlement.

The cEdge is a Catalyst 8000V Edge Router running in controller-mode.  That image is included by default
within CML, but can be downloaded from https://software.cisco.com/download/home/286327102/type with a proper
Cisco.com account and entitlement.

### Known Issues

While the `cat-sdwan-*` nodes support cloud-init day 0 configuration, the config extraction does not re-generate the cloud-init
config.  Therefore, config extraction will not work correctly on the `cat-sdwan-*` nodes.
