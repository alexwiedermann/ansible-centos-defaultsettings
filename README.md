### Install ansible

MacOSX

```
brew install ansible
```

### Create a inventory file with your machines

inventory:
```
[vm]
192.168.0.1
[vm:vars]
ansible_user=centos
ansible_ssh_private_key_file=~/.ssh/id_rsa
ansible_become=true
[defaults]
host_key_checking = False
```
