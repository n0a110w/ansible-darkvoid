# What is ansible-darkvoid? 
an ansible playbook to provision a void linux host for penetration testing and CTF challenges

It is inspired by the Shiva ansible playbook, but modified to target void linux hosts.  

1. create a minimal void linux target host (ha..)
2. install ansible on your local machine
3. clone this repo. `git clone https://github.com/n0a110w/ansible-darkvoid.git`
4. modify `inventory.ini` and replace the IP address with your void linux target
5. run the playbook. `ansible -i inventory.ini playbook.yml`


