# Linux-Infrastructure-Deployment-Automation-and-Monitoring-Lab

## 1. Project Overview

Design and deploy an enterprise-style Linux infrastructure environment using Hyper-V and Ubuntu Server. The project focuses on Linux system administration, network configuration, security hardening, infrastructure automation, and centralized monitoring.

## 2. Project Objectives

- Deploy and configure Linux virtual machines.
- Configure private networking and static IP addressing.
- Implement Linux user, group, and permission management.
- Secure remote administration using SSH and firewall rules.
- Automate server configuration using Ansible.
- Develop Bash and Python administration scripts.
- Deploy and manage Nginx.
- Implement infrastructure monitoring using Prometheus and Grafana.
- Perform troubleshooting, backup, and recovery.

## 3. Technologies and Tools

| Technology | Purpose |
|---|---|
| Hyper-V | Virtualization |
| Ubuntu Server 24.04 | Linux operating system |
| Ansible | Configuration automation |
| Bash / Python | Scripting |
| Nginx | Web services |
| Prometheus | Metrics collection |
| Grafana | Monitoring dashboards |
| SSH / UFW | Remote access and security |
| Git / GitLab | Version control and documentation |

## 4. Infrastructure Architecture

The environment consists of three virtual machines:

- **Management Server:** Ansible, SSH, Bash, and Python.
- **Web Server:** Nginx and Linux administration.
- **Monitoring Server:** Prometheus and Grafana.

```text
             WINDOWS HOST
                  |
             HYPER-V
                  |
          PRIVATE VIRTUAL NETWORK
                  |
       +----------+----------+
       |          |          |
       v          v          v
   MANAGEMENT    WEB      MONITORING
    SERVER       SERVER     SERVER
       |          |          |
    Ansible     Nginx    Prometheus
    SSH         Linux      Grafana
    Scripts     Security   Metrics
```

## 5. Implementation Phases

### Phase 1: Virtualization and Networking
- Configure Hyper-V virtual switch.
- Create private virtual network.
- Configure IP addressing.
- Allocate VM resources.

**Screenshots**
- Hyper-V Manager.
  <img width="1920" height="1080" alt="Screenshot 2026-11-11 140249" src="https://github.com/user-attachments/assets/6b03f737-9541-4c0d-aac9-6676ec7a5762" />

- Virtual switch configuration.
  <img width="1920" height="1080" alt="Screenshot 2026-11-11 140035" src="https://github.com/user-attachments/assets/02f6fe6d-e740-4100-8f58-78c2f8394c69" />

- Network configuration.
<img width="1920" height="1080" alt="Screenshot 2026-11-11 140536" src="https://github.com/user-attachments/assets/f160ec0d-9272-4b36-a780-b7afd55b1fc6" />

### Phase 2: Linux Server Deployment
- Install Ubuntu Server.
- Deploy three virtual machines.
- Configure hostnames and static IPs.
- Verify network connectivity.

**Screenshots**
- Ubuntu installation.
  <img width="1920" height="1080" alt="Screenshot 2026-11-11 142442" src="https://github.com/user-attachments/assets/e97ca441-7d7b-4557-b26a-e191f010f92a" />
<img width="1920" height="1080" alt="Screenshot 2026-11-11 144214" src="https://github.com/user-attachments/assets/934249bb-3eb9-4e80-ab18-eebd0392a91a" />

- VM configurations.
  <img width="1920" height="1080" alt="Screenshot 2026-11-11 142626" src="https://github.com/user-attachments/assets/7e719e76-5f30-4d06-85e3-23f7045de237" />

- Hostname and IP configuration.
 <img width="1920" height="1080" alt="Screenshot 2026-11-11 163119" src="https://github.com/user-attachments/assets/df71e954-2ea5-4011-b679-fc6027fe6419" />
 
- Connectivity tests.
<img width="1920" height="1080" alt="Screenshot 2026-11-11 163604" src="https://github.com/user-attachments/assets/6ee4c17f-df43-4b34-8bec-a9390fd011cd" />

### Phase 3: Linux Administration and Security
- Manage users, groups, and permissions.
- Configure SSH authentication.
- Implement UFW firewall rules.
- Manage packages, services, and logs.
- Configure disk storage.

**Screenshots**
- User and permission configuration.
- SSH authentication.
- Firewall rules.
- System and disk information.

### Phase 4: Infrastructure Automation
- Install and configure Ansible.
- Create inventory files.
- Establish SSH connectivity.
- Develop and execute automation playbooks.
- Automate package and service deployment.

**Screenshots**
- Ansible installation.
- Inventory configuration.
- Connectivity tests.
- Playbook execution.

### Phase 5: Web Services and Monitoring
- Deploy Nginx.
- Configure and test web services.
- Install Prometheus and Node Exporter.
- Configure Grafana dashboards.
- Monitor server availability and resource utilization.

**Screenshots**
- Nginx service and webpage.
- Prometheus targets.
- Node Exporter.
- Grafana dashboard.

### Phase 6: Troubleshooting and Recovery
- Troubleshoot SSH and DNS connectivity.
- Investigate Linux service failures.
- Monitor disk and system resources.
- Configure backups.
- Test recovery procedures.

**Screenshots**
- Troubleshooting commands.
- Service recovery.
- Backup configuration.
- Recovery validation.

## 6. Repository Structure

```text
enterprise-linux-infrastructure-lab/
│
├── README.md
├── architecture/
│   └── infrastructure-topology.png
├── ansible/
│   ├── inventory/
│   └── playbooks/
├── scripts/
│   ├── bash/
│   └── python/
├── monitoring/
│   ├── prometheus/
│   └── grafana/
├── documentation/
└── screenshots/
    ├── phase-1-virtualization/
    ├── phase-2-linux-deployment/
    ├── phase-3-linux-security/
    ├── phase-4-automation/
    ├── phase-5-monitoring/
    └── phase-6-troubleshooting/

```

## 7. Author

**Nadia Kroduah**

Cloud and Network Engineering | Linux Infrastructure | Cloud Administration | Automation
