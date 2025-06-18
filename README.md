network-topology-lab/
├── README.md
├── diagrams/
│   └── topology-diagram.png
├── configs/
│   ├── router1.txt
│   └── switch1.txt
└── packet-tracer/
    └── company-network.pkt
    # Network Topology Lab

A simulation of a mid-sized enterprise network using Cisco Packet Tracer. Designed to practice routing, VLANs, DHCP, and basic ACLs.

## Features
- VLAN segmentation
- DHCP Server setup
- Static and dynamic routing
- Basic firewall ACLs

## Tools
- Cisco Packet Tracer
- Wireshark (for analysis)

## Author
David Gitonga

fiber-optics-maintenance-log/
├── README.md
├── daily-logs/
│   └── 2025-06-15-log.md
├── test-results/
│   ├── otdr-sample-report.pdf
│   └── power-meter-results.csv
└── tools/
    └── troubleshooting-guide.md

  ### Location: Machakos 
- Fiber Segment: Smart OLT Configuration 
- Action: Cleaned connectors, spliced drop cable
- Tools: OTDR, Light Source, Power Meter
- Result: Power loss reduced from -25 dB to -15 dB
- Status: Resolved
  hospital-it-scripts/

├── README.md
├── bash/
│   └── auto-backup.sh
├── python/
│   └── ehr-log-analyzer.py
└── logs/
    └── backup-log-sample.txt
  #!/bin/bash
# Simple script for daily backup of hospital EHR system

DATE=$(date +%F)
SRC="/var/hospital/ehr"
DEST="/mnt/backup/ehr_$DATE"
mkdir -p $DEST
cp -r $SRC/* $DEST
echo "Backup complete for $DATE" >> /var/log/ehr_backup.log

cybersecurity-playground/
├── README.md
├── sniffing/
│   └── wireshark-analysis.pcapng
├── scanning/
│   └── nmap-scan-report.txt
├── mitigation/
│   └── firewall-rules.sh
└── notes/
    └── common-vulnerabilities.md
#!/bin/bash
# Basic iptables rules for securing a Linux server

iptables -A INPUT -p tcp --dport 22 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -j ACCEPT
iptables -A INPUT -j DROP

personal-infra-setup/
├── README.md
├── ansible-playbooks/
│   └── setup-webserver.yml
├── system-monitoring/
│   └── zabbix-config-example.conf
├── scripts/
│   └── update-logs.sh
└── docs/
    └── linux-hardening-checklist.md
- hosts: webservers
  become: yes
  tasks:
    - name: Install Apache
      apt:
        name: apache2
        state: present

      
