Installing nodejs on ubuntu
----------------------------

* manual steps
```
curl -sL https://deb.nodesource.com/setup_16.x -o /tmp/nodesource_setup.sh
sudo bash /tmp/nodesource_setup.sh
sudo apt update
sudo apt install nodejs
```
* To verify nodejs version use ` node -v `


![image](images/ansible1.png)

## ansible playbook

[refer here](https://github.com/jayainjeti/mine/blob/main/nodejs/nodejs.yaml)



Refernces :
* for get_url [refer here](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/get_url_module.html)
* for shell [refer here](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/shell_module.html#ansible-collections-ansible-builtin-shell-module)



![preview](images/ansible2.png)
