# AI-Assisted Mini SOC Lab

A hands-on cybersecurity lab for SIEM monitoring, detection engineering, SOC automation, and AI-assisted incident triage.

## Project Goal

The goal of this project is to build a small but realistic SOC-style lab that shows the full security workflow:

Logs → SIEM → Detection → Investigation → Enrichment → AI Summary → Playbook → Report

This project is not just about installing tools. The main focus is understanding how alerts are generated, how analysts investigate them, how false positives are reduced, and how AI can support SOC work safely.

## Build Strategy

This lab will start simple and expand only when extra devices teach something useful.

Rule:

Use one device unless another device adds real learning value.

The project will begin on the Razer Blade using VMware Workstation. Other physical devices will be added later only when needed.

## Planned Lab Stages

### Stage 0 — Razer Only

Set up the basic lab environment on the Razer Blade.

### Stage 1 — Razer + VMware VMs

Create the first virtual lab:

- Ubuntu Server VM
- Windows VM
- Kali Linux VM later

First target:

Razer Blade  
→ VMware Workstation  
→ Ubuntu Server VM  
→ Windows VM  
→ Wazuh Manager  
→ Wazuh Agent  
→ First file integrity monitoring alert

### Stage 2 — Add ThinkPad as Physical Kali Machine

Use the ThinkPad later as a real physical attacker/testing machine because it already has Kali Linux dual boot.

### Stage 3 — Add Mini PC as Headless Server

Use the mini PC later as an always-on Linux server, managed through SSH from the Razer.

Possible future roles:

- Wazuh server
- Docker server
- Storage box
- Monitoring box

### Stage 4 — Add Legion Only If Needed

The Legion Y540 has HDD storage, so it will not be used as the main VM host for now. It may be used later for light testing, packet capture, or secondary lab tasks.

## Planned Modules

### 0. Base Lab Setup

Set up the basic lab environment using VMware, virtual machines, snapshots, and basic networking.

### 1. Wazuh SIEM Hello World

Install Wazuh, connect a Windows endpoint, and test file integrity monitoring.

### 2. Identity Attack Detection Lab

Create identity-based detections for failed logins, password spraying, admin activity, and privilege changes.

### 3. General Detection Lab

Generate and investigate common security events such as scans, suspicious PowerShell activity, SSH failures, and file changes.

### 4. AI SOC Assistant

Use Python and AI to summarize alerts, assign risk levels, map activity to MITRE ATT&CK, and suggest analyst actions.

### 5. SOAR Automation Playbook

Build a small automation workflow to enrich alerts and recommend whether to monitor, investigate, or escalate.

### 6. AI Phishing Email Analyzer

Build a tool that analyzes suspicious emails, extracts URLs, scores risk, and creates a short analyst report.

### 7. pfSense Firewall Lab

Use pfSense to learn network segmentation, firewall rules, traffic blocking, and logging.

### 8. SafeLine WAF Lab

Use a vulnerable web app and a WAF to understand web attack detection and blocking.

### 9. Honeypot Dashboard

Deploy a honeypot to collect attack attempts and visualize activity.

### 10. Local LLM Security Assessment

Test local AI models for prompt injection, unsafe outputs, and data leakage risks.

## Hardware Plan

| Device | Use Now? | Planned Role |
|---|---|---|
| Razer Blade 15 Advanced 2022 | Yes | Main lab machine, VMware, VMs, coding, AI later |
| Lenovo Legion Y540 | Not now | Optional later, HDD makes VMs slower |
| ThinkPad T470s | Later | Physical Kali/Windows endpoint |
| Mini PC | Later | Headless always-on Linux server |

## Current Status

- GitHub repository created
- README created
- Lab planning in progress
- Starting with Razer Blade + VMware only

## Notes

This project is for defensive cybersecurity learning only.

All testing will be done in a private lab environment using owned devices and virtual machines.

No real company data, private credentials, API keys, or unauthorized systems will be used.
