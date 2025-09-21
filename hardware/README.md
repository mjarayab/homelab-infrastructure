# Network Infrastructure

## Current Network Topology

### Physical Layout
Internet → TG2482 Router → Allied Telesis Switch → 
Devices
	├── NUC 5i3 (Proxmox)
	├── NUC 6i5 (VMware)
	├── Pi 2 (OMV)
	└── Client Devices

## Current Configuration

### TG2482 ISP Router
- **Type**: DOCSIS 3.0 cable modem/router
- **WiFi**: 802.11ac
- **LAN**: 4-port gigabit
- **Network**: 192.168.1.0/24 (flat topology)
- **DHCP Range**: 192.168.1.100-192.168.1.200

### Allied Telesis Managed Switch
- **Type**: Managed gigabit Ethernet
- **Current Mode**: Basic switching (no VLANs configured)
- **Ports**: Multiple gigabit ports
- **Management**: Web interface available

## Network Services

### DNS Configuration
- **Primary DNS**: Pi-hole (when operational)
- **Upstream**: Cloudflare (1.1.1.1, 1.0.0.1)
- **Backup**: Router DNS
- **Performance**: <10ms local response time
- **Filtering**: 15-25% query blocking rate

### DHCP Management
- **Server**: TG2482 router
- **Static Assignments**: Infrastructure devices
- **Dynamic Pool**: Client devices
- **Lease Time**: 24 hours

## Planned Network Segmentation

### VLAN Strategy
- **Management VLAN 10**: Infrastructure devices 
(10.0.10.0/24)
- **Production VLAN 20**: Core services (10.0.20.0/24)
- **Development VLAN 30**: Testing and development 
(10.0.30.0/24)
- **DMZ VLAN 40**: External-facing services (10.0.40.0/24)
- **Guest VLAN 50**: Isolated guest access (10.0.50.0/24)

### Security Implementation
- **Inter-VLAN Routing**: pfSense firewall
- **Access Control**: VLAN-based policies
- **Monitoring**: Network traffic analysis
- **Intrusion Detection**: Planned implementation

## Implementation Roadmap

### Phase 1: VLAN Foundation (Months 1-2)
- Configure VLANs on Allied Telesis switch
- Deploy pfSense virtual firewall
- Implement basic inter-VLAN routing
- Migrate devices to appropriate VLANs

### Phase 2: Security Enhancement (Months 3-4)
- Firewall rules implementation
- Network monitoring deployment
- Access control policies
- Guest network isolation

### Phase 3: Advanced Features (Months 5-6)
- Network automation
- Advanced monitoring and alerting
- Performance optimization
- Disaster recovery planning

## Network Monitoring

### Current Status
- **Manual Monitoring**: Basic router dashboard
- **Performance Tracking**: Limited metrics
- **Issue Detection**: Reactive approach

### Planned Monitoring Stack
- **Grafana**: Network performance dashboards
- **Prometheus**: Metrics collection
- **SNMP Monitoring**: Switch and router metrics
- **Alert Manager**: Automated notifications

## Documentation and Change Management

### Network Documentation
- Physical topology diagrams
- IP address management (IPAM)
- VLAN configuration records
- Firewall rule documentation

### Change Control Process
- Testing in development VLAN
- Staged implementation approach
- Rollback procedures
- Performance impact assessment
