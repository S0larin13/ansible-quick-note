

## Ansible ad-hoc

### Installing packages yum 

Let us *install* alt-php80*

```
ansible app -a "yum install -y alt-php80*"
```

## List hosts

ansible -i hosts all --list-hosts

```
ansible -i hosts all -m setup
```

## Ping all hosts (module ping)

```
ansible all -i hosts -m ping
```

## Run `pwd` on shell

```
ansible all -i hosts -m shell -a "pwd" 
```

##  Create a file 

```
ansible all -m file -a "name=testfile state=touch"
```

## Ansible playbook

### Ansible playbook update centos and Plesk 

[a link](https://github.com/S0larin13/ansible-quick-note/blob/main/update_plesk_server.yml)

### Ansible playbook snaphot vphere

[a link](https://github.com/S0larin13/ansible-quick-note/blob/main/snapshot_vpshere.yml)
