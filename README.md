# TACACS-PLUS
Terminal Access Controller Access-Control System Plus (TACACS+)

# Instructions
## 1.Install TACACS+
```
sudo apt-get install tacacs+
```
## 2.Edit Configuration File
```
git clone https://github.com/codes-libertes/TACACS-PLUS.git
cp -rfpv TACACS-PLUS/tac_plus.conf /etc/tacacs+/tac_plus.conf 
```
## 3.Restart tac_plus daemon
```
sudo systemctl status tacacs_plus.service
sudo systemctl restart tacacs_plus.service
```
## 4. Add user (System Accounts will add new user 'test')
```
sudo adduser test
```

## 5. Remove user (System Accounts will remove new user 'test')
```
sudo pkill -u test
sudo deluser test
```

## 6. Change the static @IP_addr (/etc/network/interfaces)
```
ifconfig
sudo gedit /etc/network/interfaces
-----------------------------------------
auto eth0
iface eth0 inet static
        address 192.168.10.100
        netmask 255.255.255.0
        network 192.168.10.0
        broadcast 192.168.10.255
        gateway 192.168.10.254
-----------------------------------------
```
## 7. Restart network interfaces 
```
sudo /etc/init.d/networking restart
ifconfig
```

## 8. Configure Cisco Routers and Switches
https://networkjutsu.com/configuring-aaa-on-cisco-routers-switches/
