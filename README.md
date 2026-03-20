# 🖥️ Centralized Endpoint Management (ManageEngine)

## 📌 Project Overview
This project involved the deployment and configuration of **ManageEngine Endpoint Central** (formerly Desktop Central) to manage a heterogeneous environment of Windows and Linux virtual machines. The goal was to establish centralized visibility, automate inventory collection, and prepare for remote policy enforcement.



## 🛠️ Technical Stack
- **Management Server:** Windows 11 Host
- **Managed Endpoints:** Kali Linux VM, Ubuntu VM
- **Networking:** Bridged Adapter (Shared Subnet)
- **Protocols/Ports:** HTTPS (8383), Agent Communication (8020)

## 🚀 Key Implementation Steps
1. **Server Installation:** Deployed the Endpoint Central server on a Windows 11 host and configured the web console for secure HTTPS access.
2. **Network Hardening:** Configured **Windows Firewall** inbound rules to allow traffic on ports 8020 and 8383, ensuring the agents could "check-in" to the server.
3. **Agent Deployment:** - Downloaded and installed Linux agent binaries (`UEMS_LinuxAgent.bin`) on Kali and Ubuntu.
   - Handled permissions using `chmod +x` and executed installation with root privileges.
4. **Inventory Automation:** Successfully pulled real-time hardware specifications (CPU/RAM) and software versions from the remote Linux nodes.
5. **Troubleshooting:** Diagnosed and resolved "Connection Timed Out" errors by migrating VMs from NAT to **Bridged Networking** mode.

## 🔍 Managed Inventory Details
The console successfully tracked:
- OS Versions and Kernel details.
- Hardware Specs (CPU, RAM, Disk usage).
- Installed software packages for vulnerability tracking.

## 📊 Project Evidence
*(Full technical report and deployment screenshots included in the repository files)*
