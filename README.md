# LinuxUbuntuAdmin

### 1.Initial server configuration
> Add new user
  ls /home
  adduser andrei

> Give root privileges
  visudo
  add the following: andrei ALL=(ALL:ALL) ALL
  
> Disable root access
  >> backup the configuration file
     cd /etc/ssh
     cp sshd_config sshd_config.bak


### 2. Installing & Optimizing Nginx, MariaDB and PHP 7.4

### 3. NGINX configuration

### 4. SSL configuration

### 5. Fail2Ban Config
