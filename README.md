# 🍯 OTrap

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-ODefense%20%2F%20Deception-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-None%20(Standalone)-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v2.0-cyan?style=flat-square"/>
</p>

> **OTrap** is a lightweight, multi-protocol defensive honeypot. It emulates **SSH**, **HTTP**, **HTTPS**, **FTP**, and **Telnet** services to detect, log, and analyze attacker activity such as port scans, brute-force attempts, and reconnaissance.

---

## 📌 Overview

OTrap acts as a deception layer on your network. It listens on common ports and responds with realistic banners and prompts while logging every connection, credential attempt, and command. All activity is recorded with full timestamp and source IP for later analysis.

**⚠️ LEGAL NOTICE**: Deploy **ONLY** on infrastructure you own or are explicitly authorized to monitor.

---

## 🖥️ Modules

| # | Module                  | Description |
|---|-------------------------|-------------|
| **[1]** | **Start Listener**          | Launch a single honeypot on a chosen port/protocol |
| **[2]** | **Multi-Listener**          | Start multiple default services simultaneously |
| **[3]** | **Stop Listener**           | Stop one or all active listeners |
| **[4]** | **View Log**                | Browse and filter the connection log |
| **[5]** | **Live Monitor**            | Real-time connection feed |
| **[6]** | **Statistics**              | Top attacking IPs, protocol breakdown, hourly activity |
| **[7]** | **Export**                  | Save logs as JSON + CSV |
| **[8]** | **Settings**                | Configure bind IP, ports, timeouts, log file |

---

## 📊 Key Features

- **Multi-Protocol Support**: SSH, HTTP, HTTPS, FTP, Telnet + Custom
- **Realistic Responses**: Fake banners, login prompts, and error messages
- **Credential Capture**: Logs usernames and passwords from login attempts
- **Live Logging**: Real-time colored output with protocol tags
- **Statistics Dashboard**: Top attackers, protocol usage, hourly patterns
- **Export Options**: Full JSON and CSV reports
- **High Performance**: Thread pool for handling multiple connections
- **Configurable**: Bind IP, max workers, connection timeout, custom banners

---

## ⚙️ Requirements

- **Linux** (recommended)
- **Root privileges** for ports below 1024
- **No additional dependencies** — pure Python with standard library

---

## 🚀 Usage

```bash
sudo ./OTrap

📁 Output & Logging

Main Log: ohoneypot.log (JSON lines with timestamp, IP, protocol, credentials)
Export Folder: ohoneypot_results/
JSON full export
CSV summary

Live Output: Color-coded protocol tags and source IP


📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.

AUTHORISED DECEPTION & THREAT DETECTION USE ONLY
