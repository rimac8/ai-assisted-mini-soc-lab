# Lab 00 — Base Lab Setup

## Goal

Set up the basic cybersecurity lab environment before installing Wazuh, detection rules, AI tools, firewalls, or SOAR automation.

This lab is the foundation for the full AI-Assisted Mini SOC project.

## Lab Strategy

This project will start simple.

We will use the Razer Blade as the main lab machine and run the first lab using VMware Workstation.

Extra devices will only be added later if they teach something useful.

Rule:

Use one device unless another device adds real learning value.

## Devices for This Lab

| Device | Use Now? | Role |
|---|---|---|
| Razer Blade 15 Advanced 2022 | Yes | Main VM host |
| Lenovo Legion Y540 | Not now | Optional later |
| ThinkPad T470s | Later | Physical Kali or endpoint machine |
| Mini PC | Later | Headless always-on server |

## First Lab Architecture

Razer Blade  
→ VMware Workstation  
→ Ubuntu Server VM  
→ Windows VM  
→ Kali Linux VM later

## First Milestone

The first milestone is not AI or automation yet.

The first milestone is:

Ubuntu Server VM  
→ Wazuh Manager  
→ Windows VM  
→ Wazuh Agent  
→ File Integrity Monitoring alert

## Why We Are Starting This Way

Starting with only the Razer keeps the lab clean and easy to manage.

This avoids needing multiple chargers, screens, sockets, or extra networking setup before the basics are working.

Once the first SIEM setup works, we can decide whether to add the ThinkPad, mini PC, or Legion.

## VMware VM Plan

### Ubuntu Server VM

Purpose:

Wazuh Manager / SOC server later.

Planned settings:

- 2 CPU cores
- 4 GB RAM
- 60 GB disk
- NAT network first

### Windows VM

Purpose:

Endpoint/log source for Wazuh Agent.

Planned settings:

- 2 CPU cores
- 4 GB RAM
- 60 GB disk
- NAT network first

### Kali Linux VM

Purpose:

Attacker/testing machine later.

Not needed immediately.

## Current Status

- Main GitHub README updated
- Lab 00 created
- Hardware plan updated
- Starting with Razer Blade + VMware only

## Next Steps

1. Prepare the Razer Blade
2. Reduce Chrome memory usage before running VMs
3. Create VM storage folder on D drive
4. Download Ubuntu Server ISO
5. Create Ubuntu Server VM in VMware
6. Take first snapshot after clean installation

## Completed Work

### Ubuntu SOC Server VM

Created the first Ubuntu Server VM in VMware Workstation.

VM details:

- VM name: Ubuntu-SOC-Server
- OS: Ubuntu Server 24.04.4 LTS
- Username: socadmin
- Hostname: ubuntu-soc-server
- Network mode: NAT
- SSH: Enabled
- Internet test: Successful
- Basic tools installed: open-vm-tools, net-tools, curl, wget, git, unzip

### Snapshot Created

Snapshot name:

Clean Ubuntu Server - Updated + SSH Ready

Purpose:

This snapshot allows the lab to be safely restored before installing Wazuh or making major changes.
## Notes

This lab is for defensive cybersecurity learning only.

All testing will be done on owned devices and virtual machines.

No real company data, private credentials, API keys, or unauthorized systems will be used.
