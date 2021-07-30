# installing
```console
bibo318@kali:~# apt-get update
bibo318@kali:~# apt-get dist-upgrade
bibo318@kali:~# sudo apt install gvm -y # sudo apt install openvas -y
bibo318@kali:~# sudo gvm-setup
```
**user admin:password is create here, copy ur password and save it somewhere**

Once gvm-setup completes its process, the OpenVAS manager, scanner, and GSAD services should be listening:
```console
bibo318@kali:~# netstat -antp # should shows the output below
Active Internet connections (servers and established)
Proto Recv-Q Send-Q Local Address Foreign Address State PID/Program name
tcp 0 0 127.0.0.1:9390 0.0.0.0:* LISTEN 9583/openvasmd
tcp 0 0 127.0.0.1:9391 0.0.0.0:* LISTEN 9570/openvassd: Wai
tcp 0 0 127.0.0.1:9392 0.0.0.0:* LISTEN 9596/gsad
```
# using
```
bibo318@kali:~# openvas-start
bibo318@kali:~# openvas-stop
```

gvmd --create-user=kali --password=kali --role=Admin

- resource
  - [installing](https://www.kali.org/penetration-testing/openvas-vulnerability-scanning/) 
  - https://dannyda.com/2020/08/07/how-to-fix-openvas-command-not-found-in-kali-linux-2020-2a/









