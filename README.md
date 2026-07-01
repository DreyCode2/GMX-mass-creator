# GMX Account Creator & Automation Toolkit

[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Linux%20%7C%20Windows-lightgrey)]()

Enterprise-grade solution for automated GMX email account provisioning and POP3/IMAP configuration. Built for QA testing, email infrastructure validation, and legitimate bulk account management.

## 🚀 Features

- **High-performance multithreading** - Concurrent account creation with configurable thread pool
- **Advanced browser fingerprinting** - Emulates Chrome 136 TLS fingerprints to avoid detection
- **Intelligent proxy rotation** - Automatic proxy failover and rotation
- **CAPTCHA bypass** - Integration with multiple CAPTCHA solving services (CapSolver, CaptchaFox)
- **POP3/IMAP activation** - Fully automated enabling of email protocols
- **Anti-detection mechanisms** - Randomized user agents, request timing, and browser headers
- **Session persistence** - Maintains authentication state across requests
- **Comprehensive logging** - Structured logging with Loguru

## 📋 Requirements

- **VPS** (Debian 11/12, Ubuntu 20.04+) or **Windows Device**
- **Minimum Specs:** 2 vCPU, 2GB RAM (4GB recommended for high concurrency)
- **Python 3.10+** with pip
- **Active internet connection** with outbound HTTPS access
- **API Keys** (see below)

### Required API Services
- **[CapSolver](https://capsolver.com/)** - For solving POP3/IMAP activation CAPTCHAs
- **[CaptchaFox](https://captchafox.com/)** - For solving registration CAPTCHAs

## 🔧 Installation

```bash
# Clone repository
git clone https://github.com/DreyCode2/GMX-mass-creator.git
cd GMX-mass-creator

# Install Python dependencies
pip install -r requirements.txt

# Execute main.py to start
python main.py
