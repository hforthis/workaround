# BASH
{+ Commands to work +}

## Patroni + postgresql:  

Сначала посмотреть кто реплика.  
#### check list members cluster  
```/usr/local/bin/patronictl -c /etc/patroni/postgres.yml list```. 

Изменять сначала реплику!!!. 
#### change leader.  
```/usr/local/bin/patronictl -c /etc/patroni/postgres.yml switchover cluster_name```. 


## Git:  
#### add new branch  
```git checkout -b hotfix/name_new_branch```. 
  
## Linux
#### change hostname
```hostnamectl set-hostname new_name --static```. 

```hostnamectl set-hostname new_name --pretty```. 

```reboot```. 
