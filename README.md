### What is ansible-darkvoid? 

***not finished...***

- an ansible playbook to provision a void linux host for penetration testing and ctf challenges
- I recommend using [Vultr](https://www.vultr.com/?ref=7453761) because allow uploading custom ISOs

1. create a minimal void linux host
2. install ansible on your local machine
3. clone this repo. `git clone https://github.com/n0a110w/ansible-darkvoid.git`
4. modify `inventory.ini` and replace the IP address with your void linux target
5. run the playbook. `ansible -i inventory.ini playbook.yml`


## What's included? 
|name|role|
|:---|:---|
|[hashid](https://github.com/psypanda/hashID)|cracking|
|[seclists](https://github.com/danielmiessler/SecLists)|cracking|
|[hydra](https://github.com/vanhauser-thc/thc-hydra)|cracking|
|[john](https://www.openwall.com/john/)|cracking|
|[hashcat](https://hashcat.net/hashcat/)|cracking|
|---|---|
|[gobuster](https://github.com/OJ/gobuster)|web|
|[ffuf](https://github.com/ffuf/ffuf)|web|
|[wfuzz](https://github.com/xmendez/wfuzz)|web|
|[gfuzz](https://github.com/braaaax/gfuzz)|web|
|[dirb](http://dirb.sourceforge.net/)|web|
|[sqlmap](http://sqlmap.org/)|web|
|[xsser](https://github.com/epsylon/xsser)|web|
|[wafw00f](https://github.com/EnableSecurity/wafw00f)|web|
|---|---|
|[netdiscover](https://sourceforge.net/projects/netdiscover/)|recon|
|[nmap](https://nmap.org/)|recon|
|[termshark](https://github.com/gcla/termshark)|recon|
|[pspy](https://github.com/DominicBreuker/pspy)|recon|
|---|---|
|[binwalk](https://github.com/ReFirmLabs/binwalk)|re|
|[peda](https://github.com/longld/peda)|re|
|[radare2](https://github.com/radareorg/radare2)|re|
***not finished***


some online challenges include:  
- [OverTheWire](https://overthewire.org/wargames/)
- [pwnable](http://pwnable.kr/)
- [HackThebox](https://www.hackthebox.eu/)
