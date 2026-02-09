# 🧠 MISP – Important Commands Reference

This document lists the key commands used during MISP installation, configuration, and integration with Wazuh SIEM as part of the Threat Intelligence task.


## 🖥️ System Preparation & Installation

📦 Update system packages:

sudo apt update && sudo apt upgrade -y

🗄️ Install MySQL client:

sudo apt install mysql-client -y

📥 Download MISP installer:

wget https://raw.githubusercontent.com/MISP/MISP/2.4/INSTALL/INSTALL.sh

🔐 Give execution permission:

chmod +x INSTALL.sh

🚀 Run installation script:

sudo ./INSTALL.sh

# 🔥 Configure firewall for web access

sudo ufw allow 80

sudo ufw allow 443

sudo ufw enable

# 🌐 Access MISP Web Interface

Open in browser:
https:// (VM - IP Address)

# ⚙️ Edit Wazuh configuration for MISP integration
sudo nano /var/ossec/etc/ossec.conf

📂 Move to Wazuh integrations directory:

cd /var/ossec/integrations/

📥 Copy custom MISP integration script:

sudo cp custom-misp.py

🔒 Set secure permissions:

sudo chmod 750 /var/ossec/integrations/custom-misp.py

sudo chown root:wazuh /var/ossec/integrations/custom-misp.py

🔄 Restart Wazuh Manager:

sudo systemctl restart wazuh-manager

# 📊 Verify integration logs
sudo tail -f /var/ossec/logs/ossec.log
