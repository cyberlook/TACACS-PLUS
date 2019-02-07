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
By default,it's still running
```
sudo /etc/init.d/tacacs_plus status
```
or
```
ps -aux | grep tac_plus
root     25945  0.0  0.0  22232   208 ?        S    00:00   0:00 /usr/sbin/tac_plus -C /etc/tacacs+/tac_plus.conf
```

Usage: /etc/init.d/tacacs_plus {start|stop|force-stop|restart|reload|force-reload|status|check}
```

```
