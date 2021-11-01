# LinuxUbuntuAdmin

### 1.Initial server configuration
1.1 Add new user
    ls /home
    adduser andrei

1.2 Give root privileges
    visudo
    add the following: andrei ALL=(ALL:ALL) ALL
  
1.3 Disable root access
    1.3.1 backup the configuration file
          
          cd /etc/ssh
          
          cp sshd_config sshd_config.bak
          
          nano sshd_config
          
          Modify: PermitRootLogin no
          
          systemctl restart ssh

1.4 Server package updates
    
    clear
    
    sudo apt update (updates the latest packages)
    
    sudo apt upgrade (run the package upgrade)
    
    sudo apt autoremove (removed unneded packages)
    
1.5 Firewall
    Allow only ports 80,443,22
    
    1.5.1 Check if firewall is installed
    
    sudo ufw status verbose
    
    1.5.2 Install ufw and configure
    
    sudo apt install ufw
    
    sudo ufw default deny incoming
    
    sudo ufw default allow outgoing
    
    sudo ufw allow ssh
    
    sudo ufw allow http
    
    sudo ufw allow https
    
    
    
    

### 2. Installing & Optimizing Nginx, MariaDB and PHP 7.4

### 3. NGINX configuration

### 4. SSL configuration

### 5. Fail2Ban Config
