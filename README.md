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
