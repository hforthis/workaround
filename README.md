# BASH
## OC command:  
#### get rolebinding - посмотреть какой SA привязан на роль edit-0. 
```oc get RoleBinding edit-0 -o yaml```.  
#### get clusterrole - посмотреть права на роль edit. 
```oc get clusterrole edit -o yaml```.  
#### подключится к шифту от конкретного пользователя. 
```oc login --token=2222222UPNtY1111111 --server=https://server_ip:6443```.  

## Patroni + postgresql:  

Сначала посмотреть кто реплика.  
#### check list members cluster  
```/usr/local/bin/patronictl -c /etc/patroni/postgres.yml list```. 

Изменять сначала реплику!!!. 
#### change leader.  
```/usr/local/bin/patronictl -c /etc/patroni/postgres.yml switchover cluster_name```. 

#### pause cluster.  
```/usr/local/bin/patronictl -c /etc/patroni/postgres.yml pause cluster_name```.

#### resume cluster.  
```/usr/local/bin/patronictl -c /etc/patroni/postgres.yml resume cluster_name```.

## Git:  
#### add new branch  
```git checkout -b hotfix/name_new_branch```. 
  
## Linux
#### change hostname
```hostnamectl set-hostname new_name --static```. 

```hostnamectl set-hostname new_name --pretty```. 

```reboot```. 
