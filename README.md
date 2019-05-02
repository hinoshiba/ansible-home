ansible points
===

* My general ansible playbooks sample

---

## icmp check

```
ansible -m ping -i hosts 192.168.1.1 -u user
```

## syntax check

```
ansible-playbook -i inventories/production/hosts common.yml --syntax-check
```

## print tasks
```
ansible-playbook -i inventories/production/hosts common.yml --list-tasks
```
* point
	* Do not print dynamic includes by `default ansible.cfg`.

## run
```
ansible-playbook -i inventories/production/hosts common.yml --ask-become-pass
```
