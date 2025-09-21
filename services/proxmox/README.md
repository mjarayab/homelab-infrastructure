# Proxmox Virtual Environment

## Host Configuration

### Intel NUC 5i3RYK - Primary Proxmox Host
- **Hardware**: i3-5010U, 16GB DDR3L, 500GB SSD
- **Proxmox Version**: Latest stable
- **Role**: Production virtualization host
- **Uptime**: 24/7 operational target

## Current Virtual Machines and Containers

### LXC Containers
1. **Pi-hole DNS Filter**
   - **Type**: LXC Container
   - **OS**: Debian 11
   - **Resources**: 512MB RAM, 1 vCPU, 8GB storage
   - **Purpose**: Network-wide DNS filtering and ad blocking
   - **Status**: Recently reactivated, configuration in 
progress

2. **Transmission BitTorrent Client**
   - **Type**: LXC Container
   - **OS**: Debian 11
   - **Resources**: 1GB RAM, 1 vCPU, 20GB storage
   - **Purpose**: Media management and downloads
   - **Integration**: OMV storage backend

### Virtual Machines
1. **GNS3 Network Laboratory**
   - **Type**: Virtual Machine
   - **OS**: Ubuntu Desktop
   - **Resources**: 4GB RAM, 2 vCPU, 100GB storage
   - **Purpose**: CCNA practice and network simulation
   - **Status**: Active learning environment

## Resource Management

### Current Allocation
- **Total RAM**: 16GB
- **Allocated**: ~8GB (containers and VMs)
- **Available**: ~8GB for expansion
- **CPU Usage**: Low average utilization
- **Storage**: 500GB SSD with ~200GB available

### Performance Monitoring
- **Method**: Proxmox web interface monitoring
- **Metrics**: CPU, RAM, storage, network usage
- **Alerts**: Manual monitoring currently
- **Optimization**: Resource allocation based on actual 
usage

## Network Configuration

### Current Setup
- **Management Interface**: 192.168.1.x (flat network)
- **Bridge**: vmbr0 (default Proxmox bridge)
- **Container Networking**: Bridge mode to physical network
- **VM Networking**: Bridge mode with virtual NICs

### Planned Network Integration
- **VLAN Support**: Configure VLAN-aware bridge
- **Network Segmentation**: Separate management from service 
traffic
- **Security**: Isolated networks for different service 
types

## Storage Configuration

### Current Storage
- **Type**: Local SSD storage
- **Format**: EXT4 on LVM
- **Backup Strategy**: Manual snapshots
- **Capacity**: 500GB total

### Planned Storage Enhancements
- **Backup Automation**: Scheduled VM/container backups
- **External Storage**: Integration with OMV NAS
- **High Availability**: Consider shared storage for cluster

## Backup and Recovery

### Current Backup Strategy
- **VM Snapshots**: Manual before major changes
- **Container Backups**: Basic configuration documentation
- **Recovery Testing**: Limited testing performed

### Planned Improvements
- **Automated Backups**: Daily incremental backups
- **Offsite Storage**: OMV integration for backup storage
- **Recovery Procedures**: Documented disaster recovery 
plans
- **Testing Schedule**: Regular recovery testing

## Future Expansion Plans

### Cluster Development
- **Additional Nodes**: Dell T320 and T110 integration
- **Shared Storage**: Network storage implementation
- **High Availability**: VM migration capabilities
- **Load Balancing**: Service distribution across nodes

### Advanced Features
- **API Integration**: Automation scripting
- **Monitoring Integration**: Grafana dashboard development
- **Template Management**: Standard VM/container templates
- **Infrastructure as Code**: Terraform integration planning

## Learning and Development

### Skills Development
- **Proxmox Administration**: Web interface and CLI 
management
- **Virtualization Concepts**: Container vs VM optimization
- **Resource Planning**: Capacity planning and optimization
- **Networking**: Virtual networking and VLAN configuration

### Documentation Standards
- **Configuration Records**: Systematic documentation 
approach
- **Change Management**: Planned change documentation
- **Troubleshooting Guides**: Common issue resolution
- **Performance Baselines**: Resource usage tracking
