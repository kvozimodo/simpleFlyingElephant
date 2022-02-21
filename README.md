# Simple Flying Elephant
## Prerequirments
VirtualBox
```bash
sudo pacman -S virtualbox
sudo pacman -S linux516-virtualbox-host-modules    
```
Ansible
```bash
sudo pacman -S ansible
```
##Preparing VM
### On Host
Create ssh key pair
```bash
ssh-keygen -t rsa -f kuberkey.rsa
```
Copy keys to .ssh/
```bash
cp kuberkey.rsa.pub .ssh/  
cp kuberkey.rsa .ssh/ 
```
Copy public key to VM
```bash
sh-copy-id -i .ssh/kuberkey.rsa.pub kubermaster@[ip]
```

