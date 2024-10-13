# OS Security Hardening Checklist for Windows-10/11-Based Devices

## Systems of Focus

- #### [General Intro Sections]

- #### UEFI Customization and Reprogramming [Extensive Research Needed]
	- Enforcing Custom Secure Boot Keys
	- Lockdown Certain UEFI Settings & Boot Order
	- Anti-Tamper Mechanisms

- #### System Boot Security
	- Secure Boot
	- TPM Configuration (hardware-backed security)
	- General UEFI Settings (disable legacy boot, require signed firmware, etc.)

- #### Disk and Data Encryption
	- BitLocker and BitLocker To Go
	- Data Recovery Agent (DRA)
	- Disable/Lock Unused Drives (partitions too?)
	
- #### Device and Peripheral Security
	- Restrict USB Access (GPO or other methods)
	- Disable Unnecessary Peripherals (e.g. Bluetooth, etc...)
	- Device Guard (driver and application control - research)

- #### Patch Management [Remove? Less low-level]
	- Automatic Windows Update for Critical Patches
	- WSUS / Windows Update for Business Managed Patch Deployment
	- Third-party Software Patch Checks and Updates

- #### Network and Firewall Security
	- Inbound/Outbound Rules in Windows Firewall
	- Disable SMBv1 (enforce SMBv3 and higher - research)
	- Enforce TLS 1.3 (Also 1.2? - research)
	- Network Isolation / Critical Service Segmentation

- #### Registry (- Research)
	- Disable SMBv1, LMHash, other legacy protocols via registry (- research)
	- Enable LSA Protection (secure sensitve processes - research)
	- Configure RDP Settings (Auto-Run, etc. - research)

- #### Secure Network Communication
	- IPsec Configuration for Network Traffic Authentication
	- Harden DNS Settings (and DNS-over-HTTPS/DoH)
	- Disable NetBIOS and LLMNR - research

- #### Services and Features [Needed..?]
	- Remove/Disable Unnecessary Services (e.g. Print Spooler, etc... - research)
	- Remove/Disable Protocols (e.g. Telnet, etc... - research)
	- Administrator-Only Restrictions to PowerShell Remoting and WMI - research

- #### Account and Authentication Security [Needed..?]
	- Configure Password Policies
	- Remove Unnecessary Accounts
	- Credential Guard for Virtualized Environments