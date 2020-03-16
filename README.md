## What is darkvoid? 

***not finished...***

an ansible playbook to provision a void linux host for penetration testing and ctf challenges

## How to use this playbook?
```
1. create a minimal void linux host

2. install ansible on your local machine

3. clone this repo. 
git clone https://github.com/n0a110w/ansible-darkvoid.git

4. modify `inventory.ini` and replace the IP address with your void linux target

5. run the playbook. 
ansible -i inventory.ini playbook.yml
```

## What's included? 

- **cracking:**  
    - [hashid](https://github.com/psypanda/hashID), [seclists](https://github.com/danielmiessler/SecLists), [hydra](https://github.com/vanhauser-thc/thc-hydra), [john](https://www.openwall.com/john/), [hashcat](https://hashcat.net/hashcat/)  
- **web:**  
    - [gobuster](https://github.com/OJ/gobuster), [ffuf](https://github.com/ffuf/ffuf), [wfuzz](https://github.com/xmendez/wfuzz). [gfuzz](https://github.com/braaaax/gfuzz), [dirb](http://dirb.sourceforge.net/), [sqlmap](http://sqlmap.org/), [xsser](https://github.com/epsylon/xsser), [wafw00f](https://github.com/EnableSecurity/wafw00f) 
- **recon:**  
    - [netdiscover](https://sourceforge.net/projects/netdiscover/), [nmap](https://nmap.org/), [termshark](https://github.com/gcla/termshark), [pspy](https://github.com/DominicBreuker/pspy)
- **re:**  
    - [binwalk](https://github.com/ReFirmLabs/binwalk), [peda](https://github.com/longld/peda), [radare2](https://github.com/radareorg/radare2)

***not finished***

---

popular online challenges:  
- [OverTheWire](https://overthewire.org/wargames/)
- [pwnable](http://pwnable.kr/)
- [HackThebox](https://www.hackthebox.eu/)

---

*I recommend using [Vultr](https://www.vultr.com/?ref=7453761) to deploy your instances because they allow uploading of custom ISOs*
