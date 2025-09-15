# Pi-hole Production Service

## Overview
DNS filtering and ad-blocking service deployed on Proxmox infrastructure 
using LXC containerization.

## Infrastructure Details
- **Platform**: Proxmox VE on Intel NUC 5i3
- **Container Type**: LXC (lightweight virtualization)
- **OS**: Ubuntu 22.04 LTS
- **Resources**: 1GB RAM, 8GB storage
- **Network**: Bridged mode with static IP assignment

## Service Management
- **Current Status**: Active (reactivated September 2024)
- **Lifecycle Approach**: Hibernation during non-critical periods for 
resource efficiency
- **Maintenance**: Regular updates of Pi-hole core and blocklists
- **Monitoring**: Web interface accessible at http://pihole.local/admin

## Technical Implementation
- Automated deployment via Proxmox LXC templates
- Custom blocklist configuration for enhanced filtering
- Upstream DNS: Cloudflare (1.1.1.1) with fallback to Quad9
- DHCP integration with network infrastructure

## DevOps Practices Applied
- Infrastructure as Code mindset for reproducible deployments
- Service lifecycle management (start/stop/hibernate)
- Proactive maintenance and security updates
- Documentation-first approach for operational procedures

## Recent Updates (September 2024)
- Updated Pi-hole to latest stable version
- Refreshed all blocklist subscriptions  
- Updated underlying Ubuntu container to latest patches
- Verified DNS resolution performance and filtering effectiveness

## Learning Objectives
- Advanced Python scripting for automation
- Enhanced Bash scripting for service management
- Integration with monitoring solutions (Prometheus/Grafana)
- GitOps practices for configuration management
