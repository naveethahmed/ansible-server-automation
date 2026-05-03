# ⚙️ Server Configuration and Automation using Ansible

## 📌 Overview
Automated Linux server setup and configuration using Ansible 
playbooks. Installs and configures Nginx, Docker, UFW firewall 
and deploys a web application across multiple AWS EC2 instances.

## 🏗️ Architecture
Ansible Control Node → Inventory File → Target EC2 Servers
→ Web Servers (Nginx)
→ DB Servers

## 🛠️ Tools & Technologies
| Tool | Purpose |
|------|---------|
| Ansible | Configuration Management |
| AWS EC2 | Target Servers (Ubuntu) |
| Nginx | Web Server |
| Docker | Containerization |
| UFW | Firewall Management |

## 📂 Project Structure
ansible-server-automation/
├── playbook.yml     # Main automation playbook
├── inventory        # Target server definitions
└── README.md        # Project documentation

## ⚙️ Tasks Automated
- ✅ System packages update and upgrade
- ✅ Nginx installation and configuration
- ✅ Docker installation
- ✅ UFW Firewall setup (SSH port 22, HTTP port 80)
- ✅ Web application deployment
- ✅ Service verification

## 🚀 How to Run
```bash
# Clone the repository
git clone https://github.com/naveethahmed/ansible-server-automation

# Test connection to servers
ansible all -i inventory -m ping

# Run the playbook
ansible-playbook -i inventory playbook.yml

# Run with verbose output
ansible-playbook -i inventory playbook.yml -v
```

## 💡 Key Concepts Demonstrated
- Agentless automation with SSH
- Idempotent configuration management
- Multi-server inventory management
- Role-based task organization
- Service management with systemd

## 👨‍💻 Author
**Naveeth Ahmed N** | DevOps Engineer  
📧 naveethahmedn@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/naveeth-ahmed-a44181313)
