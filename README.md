# Homelab Infrastructure - DevOps Learning Journey

## Project Overview

This repository documents my systematic transition from logistics coordination to DevOps engineering, showcasing real infrastructure implementations, hands-on learning progression, and practical application of enterprise methodologies. All content represents actual deployments and honest skill assessment rather than theoretical knowledge claims.

## Current Infrastructure

### Production Environment (24/7 Operation)

- **Intel NUC 5i3RYK**: Proxmox VE host running Pi-hole DNS (1+ year uptime), Transmission, GNS3
- **Intel NUC 6i5SYK**: VMware development environment with pfSense security labs
- **Raspberry Pi 2**: OpenMediaVault NAS serving Plex media and file shares
- **Network**: TG2482 ISP router + Allied Telesis managed switch (flat topology, VLAN segmentation planned)

### Standby Equipment

- **Dell PowerEdge T320**: Planned Kubernetes master node deployment
- **Dell PowerEdge T110 II**: Planned Kubernetes worker node

## Active Services

1. **Pi-hole** (LXC): Network-wide DNS filtering, household production service
1. **Transmission** (LXC): BitTorrent client with OMV storage integration
1. **GNS3** (VM): Network simulation for CCNA practice
1. **pfSense** (VM): Virtual firewall for advanced networking concepts
1. **Plex**: Media streaming server on OMV
1. **File Shares**: SMB/CIFS cross-platform access and backups

## Professional Background

### Intel Corporation (1998-2005)

**Career Progression**: Manufacturing Technician → Process Engineering Technician → Process Engineer

- **Process Engineering Excellence**: Technology transfers from US operations to Costa Rica facility
- **Team Training & Development**: Led training programs for 50+ technicians across multiple process areas
- **Quality Systems Leadership**: ISO 9001/14001 internal auditor, systematic problem-solving methodology
- **Equipment Reliability**: Achieved 90%+ availability through preventive maintenance and process optimization
- **Methodology Foundation**: Seven Steps root cause analysis, statistical process control, continuous improvement culture

### Tecnorótulos (2005-2022)

**Role**: Founder & Technical Director

- **Company Type**: Corporate signage design, fabrication, and installation services
- **Scale Achievement**: Grew from startup to 15-employee company serving major corporate clients
- **Major Clients**: FIFCO (Costa Rica Brewery), Musmanni (bakery chain), Four Seasons Resort, Banco Lafise
- **Technical Operations**: Project management, team leadership, client relationship management
- **Business Skills**: P&L responsibility, vendor relationships, process optimization, quality control

### Grupo Favarcia (2025-Present)

**Position**: Logistics Coordinator

**Operational Transformation Through Systematic Methodology**

Applying Intel Seven Steps problem-solving approach to warehouse operations, driving measurable improvements in team performance and operational efficiency.

**Process Improvement Initiatives:**

- **Workflow Optimization**: Systematic analysis and documentation of inventory management processes
- **Operational Planning**: Implementation of proactive coordination systems and daily planning procedures
- **Efficiency Analysis**: Identification and resolution of logistics bottlenecks through data-driven approach
- **Procedure Standardization**: Development of documented best practices for consistent execution
- **Technology Evaluation**: Assessment of automation opportunities for manual process improvement

**Team Leadership & Development:**

- **Collaborative Environment**: Leading 8-10 warehouse associates toward systematic problem-solving culture
- **Communication Enhancement**: Established effective coordination between management and operations teams
- **Recognition Systems**: Daily positive reinforcement and performance acknowledgment implementation
- **Cross-Training Programs**: Knowledge sharing initiatives for operational flexibility
- **Continuous Improvement**: Shift from reactive operations to proactive issue identification and resolution

**Measurable Outcomes:**

- Enhanced team collaboration and communication effectiveness across shifts
- Systematic problem-solving methodology replacing ad-hoc reactive approaches
- Improved operational planning reducing last-minute scheduling challenges
- Documentation of procedures enabling knowledge transfer and consistent quality
- Increased team engagement through recognition and clear communication

**Skills Applied:**

- Seven Steps methodology for root cause analysis and systematic improvement
- Process documentation and standard operating procedure development
- Change management and cultural transformation leadership
- Cross-functional communication and stakeholder coordination
- Performance metrics development aligned with operational reality

**Professional Development Integration:**
This role demonstrates practical application of process engineering principles to logistics operations, leadership development in operational environments, and systematic problem-solving - competencies directly transferable to DevOps team leadership and operational excellence roles.

## Skills Development

### Current Level (Honest Assessment)

- **Virtualization**: Proxmox basic-intermediate, VMware basic-intermediate
- **Operating Systems**: Linux basic-intermediate (Ubuntu, CentOS, Debian)
- **Networking**: CCNA theory in progress (Universidad Nacional), flat network operational experience
- **Scripting**: Python beginner level, bash basics
- **Version Control**: Git/GitHub professional workflow established
- **Containers**: Docker theoretical knowledge, practical implementation planned

### Active Learning

- **CCNA Certification**: Universidad Nacional Cisco Networking Academy program
- **Python Development**: Hands-on learning through vehicle control system project
- **Container Technology**: Docker and Kubernetes study with planned homelab implementation
- **Infrastructure Monitoring**: Grafana and Prometheus preparation
- **Infrastructure as Code**: Terraform and Ansible conceptual learning

## Development Roadmap

### Priority 1: Foundation (Months 1-3)

- VLAN network segmentation implementation
- Dell T320 server deployment with storage configuration
- Docker service containerization
- CCNA certification completion
- Python fundamentals through practical application

### Priority 2: Intermediate (Months 4-6)

- Kubernetes cluster deployment (T320 + T110)
- Monitoring stack implementation (Grafana + Prometheus)
- Vehicle control system development and production deployment
- Automated backup solution implementation

### Priority 3: Advanced (Months 7-12)

- CI/CD pipeline basic implementation
- Infrastructure as Code adoption (Terraform/Ansible basics)
- Advanced networking features (VPNs, advanced firewall rules)
- High availability concepts and disaster recovery planning

## Real-World Project: Vehicle Control System

### Business Context

Development of web-based vehicle inspection and control system for family business operations, replacing manual paper forms with digital workflow and historical tracking.

### Technical Implementation

- **Backend**: Python Flask framework + PostgreSQL database
- **Frontend**: Responsive web interface for mobile field use
- **Features**: Vehicle registration, pre/post-trip inspections, damage documentation with photos, automated PDF report generation
- **Deployment**: Self-hosted on homelab infrastructure
- **Collaboration**: Two-developer team using professional Git workflow

### Project Value

- **Portfolio Demonstration**: Full-stack development with real business requirements
- **Practical Learning**: Python, databases, web frameworks, deployment practices
- **Business Impact**: Operational efficiency improvement and compliance documentation
- **Professional Skills**: Requirements gathering, stakeholder management, project delivery

## Career Transition Strategy

### Target Position

DevOps Engineer / Team Lead with $1500-2500 USD compensation range in Costa Rica or remote international opportunities.

### Realistic Timeline

18-24 months for systematic skill development and portfolio building, emphasizing learning journey transparency over premature expertise claims.

### Competitive Advantages

- **Real Infrastructure**: Physical homelab providing production-like experience vs cloud-only implementations
- **Engineering Foundation**: Intel process improvement methodology and quality systems background
- **Business Experience**: P&L responsibility and team leadership from 17-year company ownership
- **Current Operations**: Active application of systematic problem-solving in logistics environment
- **Learning Transparency**: Honest skill assessment and documented progression demonstrating growth mindset

### Portfolio Development Approach

- **GitHub Repository**: Professional documentation of actual implementations with visual evidence
- **Learning Journey**: Daily study notes and systematic skill progression documentation
- **Real Projects**: Business application development demonstrating practical capability
- **Professional Standards**: Enterprise-level documentation quality and honest competency representation

## Success Metrics

### Technical Competency

- Service uptime and reliability (99%+ target for production services)
- Systematic documentation completeness and professional presentation
- Certification achievement (CCNA completion, future container certifications)
- Project implementation success with measurable business value

### Professional Development

- GitHub repository activity and quality (consistent commits, professional documentation)
- LinkedIn profile optimization and professional networking growth
- Job market engagement and interview conversion rates
- Skill validation through practical implementations and peer feedback

### Business Value Creation

- Vehicle control system operational deployment and stakeholder satisfaction
- Homelab cost efficiency and resource optimization
- Family business operational improvements through technology application
- Process improvement documentation and knowledge transfer capability

## Repository Structure

```
homelab-infrastructure/
├── README.md                    # This comprehensive documentation
├── services/                    # Production service documentation
│   └── pihole-production.md    # Pi-hole deployment and configuration
├── hardware/                    # Physical infrastructure inventory
│   ├── inventory.md            # Complete hardware specifications
│   └── photos/                 # Visual documentation of equipment
├── network/                     # Network topology and planning
├── study-notes/                # Learning journey documentation
│   ├── dia-1-2-git-fundamentals.md
│   ├── dia-3-professional-documentation.md
│   ├── day-4-repository-infrastructure-recovery
│   └── seven-steps-portfolio-analysis.md
├── labs/                       # Hands-on learning implementations
│   └── README.md              # Lab environment documentation
└── development/               # Development learning path
    └── README.md              # Programming skill progression
```

## Learning Methodology

### Honest Assessment Principle

All skill claims represent actual demonstrated capability rather than aspirational knowledge. Portfolio emphasizes learning progression and growth mindset over false expertise claims.

### Systematic Approach

- **Real Implementations**: Physical infrastructure deployments vs tutorial completion
- **Documentation Standards**: Professional technical writing for portfolio value
- **Progressive Complexity**: Basic operations → intermediate → planned advanced features
- **Business Application**: Practical projects with real stakeholders and requirements

### Knowledge Validation

- **Certification Path**: CCNA (in progress) → Docker/Kubernetes certifications (planned)
- **Practical Deployment**: Operational services demonstrating hands-on capability
- **Peer Review**: Code review practices and collaborative development
- **Market Feedback**: Recruiter and industry professional engagement

## Current Focus

### Week 1: Git & GitHub Mastery (Days 1-7)

- ✅ Professional Git workflow and branching strategy
- ✅ Comprehensive repository documentation
- ✅ Study notes systematic organization
- 🔄 Visual evidence implementation (hardware photography)
- 📋 Advanced Git features and professional polish

### Immediate Priorities

1. Complete CCNA certification through Universidad Nacional program
1. Implement VLAN network segmentation for security and organization
1. Deploy Dell T320 server with storage configuration
1. Begin Docker containerization of existing services
1. Continue vehicle control system development

## Technical Documentation Standards

All documentation in this repository follows professional standards:

- **Accuracy**: Honest representation of current capabilities and limitations
- **Completeness**: Sufficient technical detail for knowledge transfer and reproduction
- **Clarity**: Explanations accessible to various technical audience levels
- **Professional Presentation**: Enterprise-level documentation quality for career development
- **Continuous Updates**: Regular refinement based on learning progression and implementation

## Contact & Collaboration

Open to feedback, mentorship, and professional networking within the DevOps community. This repository represents an ongoing learning journey and commitment to systematic skill development with transparent documentation of both successes and challenges.

-----

**Last Updated**: October 2025  
**Repository Status**: Active development with consistent weekly commits  
**Learning Phase**: Foundation building with CCNA certification and Docker implementation focus