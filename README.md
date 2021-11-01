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


### 2. Installing & Optimizing Nginx, MariaDB and PHP 7.4

### 3. NGINX configuration

### 4. SSL configuration

### 5. Fail2Ban Config
