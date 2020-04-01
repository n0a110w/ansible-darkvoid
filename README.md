## What is darkvoid? 

an ansible playbook to provision a void linux host for penetration testing and ctf challenges

## Dependencies?
#### Client (local):
 - git, ansible, ansible-playbook
#### Target:
 - void linux with python3 installed 
   - *(it appears the golang toolchain requires glibc void to compile...let me know if you get it working on x86_64 musl)*

## How to use this playbook?

```
1. clone this repo locally 
git clone https://github.com/n0a110w/ansible-darkvoid.git

2. modify `inventory.ini` and replace the IP address with your void linux target(s)
# vi one-liner (though probably slower than just vi *edit* shift zz)
vi -c '%s/127.0.0.1/target.i.p.addr/' inventory.ini -c 'wq'

3. run the playbook. 
ansible -i inventory.ini playbook.yml

that's it. 
login to the system and enjoy.
```

## What's included? 

- **cracking:**  
    - [hashid](https://github.com/psypanda/hashID), [seclists](https://github.com/danielmiessler/SecLists), [hydra](https://github.com/vanhauser-thc/thc-hydra), [john](https://www.openwall.com/john/), [hashcat](https://hashcat.net/hashcat/)  
- **web:**  
    - [gobuster](https://github.com/OJ/gobuster), [ffuf](https://github.com/ffuf/ffuf), [wfuzz](https://github.com/xmendez/wfuzz). [gfuzz](https://github.com/braaaax/gfuzz), [dirb](http://dirb.sourceforge.net/), [sqlmap](http://sqlmap.org/), [xsser](https://github.com/epsylon/xsser), [wafw00f](https://github.com/EnableSecurity/wafw00f) 
- **recon:**  
    - [netdiscover](https://sourceforge.net/projects/netdiscover/), [nmap](https://nmap.org/), [termshark](https://github.com/gcla/termshark), [pspy](https://github.com/DominicBreuker/pspy)
- **reverse engineering:**  
    - [binwalk](https://github.com/ReFirmLabs/binwalk), [peda](https://github.com/longld/peda), [radare2](https://github.com/radareorg/radare2)

*thank you to the void package maintainers who make a lot of these tools available via the xbps repo. that helps tremendously.*

---

popular online challenges:  
- [OverTheWire](https://overthewire.org/wargames/)
- [pwnable](http://pwnable.kr/)
- [HackThebox](https://www.hackthebox.eu/)

---

*I recommend using [Vultr](https://www.vultr.com/?ref=7453761) to deploy your instances*
