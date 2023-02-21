##Test ssh
`ssh ci@192.168.56.12`

##Test ping cmd
`ansible all -i inventory.yml -m ping -u ci`
with: 
1. Group: `all` 
2. Inventory file : `inventory.yml`
3. Module: `ping` 
4. User: `ci`

##Test ping cmd
`ansible all -i inventory.yml -m shell -a "pwd" -u ci`

1. Group: `all` 
2. Inventory file : `inventory.yml`
3. Module: `shell` 
4. User: `ci`
5. Cmd: `pwd`

#Run ansible-playbook:
`ansible-playbook -i inventory.yml playbook.yml`
1. Inventory file : `inventory.yml`
2. Playbook file: `playbook.yml`