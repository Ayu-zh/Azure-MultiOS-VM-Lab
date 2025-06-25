# Azure Multi-OS VM Lab Environment

This project deploys a cloud-based lab on Azure with one Linux (Ubuntu 22.04) and one Windows (Server 2022) VM, showcasing skills for a Cloud Admin Intern role at Penthara Mohali.

[![Azure](https://img.shields.io/badge/Azure-Cloud-blue)](https://azure.microsoft.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)

## Features
- **VM Deployment**: Linux and Windows VMs via ARM templates.
- **Networking**: VNet with NSG for SSH (port 22) and RDP (port 3389).
- **Remote Access**: SSH for Linux, RDP for Windows.
- **Configuration**: NGINX on Linux, IIS on Windows.
- **Monitoring**: Azure Monitor for VM health.
- **Automation**: VM startup/shutdown schedule.

## Repository Structure
- `arm-templates/`: VNet, Linux, and Windows VM templates.
- `scripts/`: SSH key generation and VM scheduling scripts.
- `docs/`: Deployment guide, architecture diagram, cost management.
- `screenshots/`: Evidence of SSH, RDP, and monitoring.

## Setup Instructions
1. **Prerequisites**:
   - Azure for Students account.
   - Azure Cloud Shell or CLI/PowerShell.
   - SSH and RDP clients.
2. **Deployment**:
   - Follow `docs/deployment-guide.md`.
   - Use `arm-templates/` for VNet and VMs.
   - Run `scripts/` for SSH and automation.
3. **Verification**:
   - SSH to Linux VM, verify NGINX.
   - RDP to Windows VM, verify IIS.
   - Check Azure Monitor metrics.
4. **Cleanup**:
   - Run: `Remove-AzResourceGroup -Name MultiOSLabRG -Force`

## Screenshots (not updated)
- [Linux VM SSH](screenshots/linux-vm-ssh.png)
- [Windows VM RDP](screenshots/windows-vm-rdp.png)
- [Azure Monitor](screenshots/azure-monitor.png)

## Skills Demonstrated
- **VM Provisioning**: ARM templates for infrastructure-as-code.
- **Scripting**: Bash and PowerShell automation.
- **Networking**: VNet and NSG configuration.
- **Multi-OS**: Linux and Windows management.
- **Azure Management**: Monitoring and automation.
- **Resource Optimization**: Cost-saving strategies.

## Cost Management
See `docs/cost-management.md` for staying within Azure for Students limits.

## Contact
[LinkedIn](https://www.linkedin.com/in/ayush-priyadarshi-894836167/) | 

---
Built with Azure, PowerShell, and Bash.
