# Hardware Infrastructure

## Current Production Hardware

### Intel NUC 5i3RYK - Proxmox Host
- **CPU**: Intel i3-5010U (2.1GHz, 2C/4T)
- **RAM**: 16GB DDR3L
- **Storage**: 500GB SSD
- **Role**: Primary virtualization host
- **Status**: 24/7 operational

### Intel NUC 6i5SYK - Development Environment  
- **CPU**: Intel i5-6260U (2.9GHz, 2C/4T)
- **RAM**: 16GB DDR4
- **Storage**: 500GB SSD
- **Role**: VMware development and testing
- **Status**: Active development

### Raspberry Pi 2 - NAS
- **CPU**: ARM Cortex-A7 (900MHz)
- **RAM**: 1GB
- **Storage**: 2TB SSD via USB3
- **OS**: OpenMediaVault
- **Role**: Network storage and Plex server
- **Status**: Production

## Expansion Hardware (Standby)

### Dell PowerEdge T320
- **CPU**: Xeon socket (expandable)
- **RAM**: 16GB ECC (expandable to 192GB)
- **Storage**: No drives currently
- **Network**: Dual gigabit
- **Planned Role**: Kubernetes master node

### Dell PowerEdge T110 II
- **CPU**: Xeon socket
- **RAM**: 16GB ECC (expandable to 32GB)
- **Planned Role**: Kubernetes worker node

## Future Infrastructure - Recently Acquired

### JONSBO Chasis NAS N1 Mini-ITX
- **Form Factor**: Mini-ITX compatible
- **Storage Capacity**: 5+1 drive bays
- **Cooling**: Integrated ventilation system
- **Construction**: Aluminum with steel reinforcement
- **Status**: Acquired September 2025, planning phase
- **Evaluation**: NAS upgrade vs dedicated services node vs 
Kubernetes expansion

## Network Infrastructure

### Current Setup
- **ISP Router**: TG2482 (DOCSIS 3.0, WiFi AC)
- **Switch**: Allied Telesis managed gigabit
- **Topology**: Flat network (192.168.1.0/24)
- **Planned**: VLAN segmentation

## Power and Environmental

- **Power Budget**: ~200W total current consumption
- **Cooling**: Passive for NUCs, active for servers
- **UPS**: Planning phase
- **Rack**: Ready for rack-mount deployment
