# AI-Assisted Mini SOC Lab

A hands-on cybersecurity lab for SIEM monitoring, detection engineering, SOC automation, and AI-assisted incident triage.

## Project Goal

The goal of this project is to build a small but realistic SOC-style lab that shows the full security workflow:

Logs → SIEM → Detection → Investigation → Enrichment → AI Summary → Playbook → Report

This project is not just about installing tools. The main focus is understanding how alerts are generated, how analysts investigate them, how false positives are reduced, and how AI can support SOC work safely.

## Planned Modules

### 0. Base Lab Setup

Set up the basic lab environment using virtual machines and physical devices.

### 1. Wazuh SIEM Hello World

Install Wazuh, connect an endpoint, and test file integrity monitoring.

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

## Current Status

Project repository created.  
First lab setup is in progress.

## Hardware Available

- Razer Blade 15 Advanced 2022
- Lenovo Legion Y540 with GTX 1660 Ti and 16GB RAM
- Lenovo ThinkCentre mini PC
- ThinkPad T470s

## Notes

This project is for defensive cybersecurity learning only.  
All testing will be done in a private lab environment using owned devices and virtual machines.
