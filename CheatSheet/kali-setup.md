# todo:
- [ ] https://github.com/DominicBreuker/pspy
# general
```console
bibo318@parrot:~$ sudo apt-get install -y gobuster
bibo318@parrot:~$ sudo apt-get install -y python3-pip
bibo318@parrot:~$ sudo apt-get install -y openvpn
bibo318@parrot:~$ sudo apt-get install -y seclists # seclist wordlist!!
bibo318@parrot:/opt$ sudo wget https://raw.githubusercontent.com/Anon-Exploiter/SUID3NUM/master/suid3num.py
bibo318@parrot:~$ sudo apt-get install -y golang # go
bibo318@parrot:~$ sudo apt-get install -y steghide
bibo318@parrot:~$ sudo apt-get install -y remmina # rdp tool
bibo318@parrot:~$ sudo apt-get install -y evolution # email client app
```
or
```console
bibo318@parrot:~$ sudo apt-get install -y gobuster python3-pip openvpn seclists golang steghide steghide remmina
```
# terminator
- [unlimited-scroll](https://askubuntu.com/questions/618464/unlimited-scroll-in-terminator) 
```console
$ sudo apt-get install terminator
$ nano terminator/config # Open the terminator config file
```
under the `[profiles]` entry add those lines
```
  [[default]]
    scrollback_infinite = True
```
Now save and exit then restart your terminator. enjoy

# pymap
```console
bibo318@parrot:/opt$ sudo wget https://raw.githubusercontent.com/gu2rks/pymap/master/pymap.py
bibo318@parrot:/opt$ sudo chmod +x pymap.py 
```
# impacket
```console
$ sudo git clone https://github.com/SecureAuthCorp/impacket.git
$ cd impacket && pip3 install -r requirements.txt
$ sudo python3 setup.py install
```
# privilege-escalation-awesome-scripts-suite
```console
$ sudo git clone https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite.git
$ sudo mkdir privesc
bibo318@parrot:/opt$ sudo cp privilege-escalation-awesome-scripts-suite/winPEAS/winPEASexe/winPEAS/obj/x64/Release/winPEAS.exe privesc/winPEAS-x64.exe
bibo318@parrot:/opt$ sudo cp privilege-escalation-awesome-scripts-suite/winPEAS/winPEASexe/winPEAS/obj/x86/Release/winPEAS.exe privesc/winPEAS-x86.exe
bibo318@parrot:/opt$ sudo cp privilege-escalation-awesome-scripts-suite/winPEAS/winPEASbat/winPEAS.bat privesc/
bibo318@parrot:/opt$ sudo cp privilege-escalation-awesome-scripts-suite/linPEAS/linpeas.sh privesc/
```

# Sipvicious
- https://github.com/EnableSecurity/sipvicious
```console
$ sudo pip3 install sipvicious
```

# Empire
```console
$ cd /opt
$ git clone https://github.com/BC-SECURITY/Empire.git
$ cd Empire    
$ sudo ./setup/install.sh    
```

# Starkiller
- Empire is requried
## Installing
```console
$ cd /opt
$ # Download an up to date version of starkiller from the BC-Security Github repo - https://github.com/BC-SECURITY/Starkiller/releases 
$ chmod +x starkiller-1.X.X.AppImage
$ sudo ./starkiller-1.X.X.AppImage --no-sandbox
```
## Setting Up Starkiller
```console
$ cd /opt/Empire
$ sudo ./empire --rest # on 1st terminal run empire
$ sudo ./starkiller-1.X.X.AppImage --no-sandbox # 2nd run starkiller!
```
Default Credentials:
- uri: 127.0.0.1:1337
- user: empireadmin
- pass: password123
