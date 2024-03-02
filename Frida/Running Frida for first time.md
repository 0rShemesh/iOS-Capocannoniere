Never used Frida because I hate JavaScript
So after [installing on the device](https://frida.re/docs/ios/) by adding the repo:
https://build.frida.re

and on my Linux machine by typing:
```bash
pip install frida-tools
```


Lets tunnel to the Frida port:
```bash
ssh -N mobile@${device_ip} -L 27042:127.0.0.1:27042
```
Yay now lets just try frida by running:
```
frida-ps -R
```
![](../Photos/Pasted%20image%2020240302155955.png)
works! 

