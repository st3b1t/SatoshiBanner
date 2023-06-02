# Satoshi.motd

Satoshi tribute for your Full Node SSH server motd(message of the day) or banner file

## Install

1) login in your full node machine and run

```bash
curl -s https://raw.githubusercontent.com/st3b1t/Satoshi.motd/main/times.txt | sudo tee /etc/motd.txt > /dev/null
```

low height version

```bash
curl -s https://raw.githubusercontent.com/st3b1t/Satoshi.motd/main/times-short.txt | sudo tee /etc/motd.txt > /dev/null
```

2) as root edit `/etc/ssh/sshd_config` uncomment or add the option `PrintMotd yes` and restart ssh server

```
service ssh reload
```


## Result

![the times](times.gif)


### Short version

![the times](times-short.png)

# License

MIT License

Copyright (c) 2023 st3b1t

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
