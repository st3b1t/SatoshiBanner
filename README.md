# Satoshi.motd

Satoshi tribute for your Full Node SSH server motd(message of the day) or banner file

## Install

login in your full node machine and run

```bash
curl -s https://raw.githubusercontent.com/st3b1t/Satoshi.motd/main/times.txt | sudo tee /etc/motd.txt > /dev/null
```

as root edit `/etc/ssh/sshd_config` uncomment or add the option `PrintMotd yes` and restart ssh server

```
service ssh reload
```

login in full node again

## Result

![the times](times.gif)
