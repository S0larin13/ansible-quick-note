- 👋 Hi, I’m @S0larin13
- 👀 I’m interested in ansible, grafana, ...
- 🌱 I’m currently learning aws, awx...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
moro13/moro13 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


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

[a link](https://github.com/S0larin13/ansible-quick-note/blob/main/update_plesk_server.yml)
