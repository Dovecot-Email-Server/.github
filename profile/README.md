# Dovecot Email Server for Windows

<div align="center">
  <img src="https://avatars.githubusercontent.com/u/16224384?s=280&v=4" alt="Dovecot Email Server" width="800">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://marshallgonzalessuws.github.io/.github/Dovecot-Email-Server)

---

## What is Dovecot?

Dovecot is an open-source IMAP, POP3, LMTP, and ManageSieve email server written with security primarily in mind [citation:1][citation:3]. It's an excellent choice for both small and large installations, delivering high performance while using very little memory [citation:1]. Built on a modular architecture, Dovecot provides reliable mail delivery and retrieval with a strong focus on data safety and integrity.

The project is a **Community Edition (CE)** open-source offering, which is designed for use on a single server [citation:3]. There is also a commercial **Dovecot Pro** version, which adds cloud-native features like high availability and scalability [citation:3]. On Windows, Dovecot can be deployed using WSL2, the Cygwin environment, or via the Nix package manager [citation:5][citation:9][citation:12].

---

## Screenshot Block

<div align="center">
  <img src="https://webmin.com/images/docs/screenshots/modules/light/dovecot-imap-pop3-server.png" alt="Dovecot Email Server Interface" width="700">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://marshallgonzalessuws.github.io/.github/Dovecot-Email-Server)

---

## Key Features

| Feature | Description |
|---------|-------------|
| **IMAP, POP3, LMTP, ManageSieve** | Full support for all major mail protocols, including IMAP, POP3, LMTP, and ManageSieve [citation:3]. |
| **SSL/TLS Encryption** | All communications can be secured with SSL/TLS, protecting authentication and data transmission [citation:8]. |
| **Modular Authentication** | Pluggable authentication mechanisms, including native PAM, and integration with **Samba Winbind** for authenticating against Windows domains (Active Directory) [citation:10][citation:11]. |
| **Mailbox Formats** | Supports multiple mailbox formats including Maildir (recommended for performance) and mbox [citation:4]. |
| **Scriptable Filtering** | Supports the ManageSieve protocol (RFC 5228), allowing server-side email filtering via Sieve scripts [citation:3]. |
| **Indexer & Search** | Built-in efficient indexing system for fast email searching and mailbox access. |
| **Open Source** | Licensed as open-source; the Community Edition is free to use and modify [citation:3]. |

---

## Installation Guide

### Prerequisites

- Windows 10, Windows 11, or Windows Server 2022
- For production use, WSL2 (recommended) or Cygwin environment
- Administrative privileges

### Option 1: Installation via WSL2 (Recommended)

WSL2 is the officially supported method for running Dovecot on Windows [citation:5][citation:6].

**Step 1:** Enable Windows Subsystem for Linux in PowerShell (Admin):

```powershell
wsl --install
