# ansible

#This is my Ansible Repo

# -----HELP-----

##		Connection Test:
###			ansible all -m ping

##  		List all of the hosts in the inventory
###	    		ansible all --list-hosts

##    		Gather facts about your hosts
###    			ansible all -m gather_facts

##    		Gather facts about your hosts, but limit it to just one host
###    			ansible all -m gather_facts --limit HOST-IP
 		
## 		Tell ansible to use sudo (become)
###			ansible all -m apt -a update_cache=true --become --ask-become-pass
		
##		Install a package via the apt module
###			ansible all -m apt -a name=vim-nox --become --ask-become-pass  -> name= apt Software
		
##		Install a package via the apt module, and also make sure it’s the latest version available
###			ansible all -m apt -a "name=snapd state=latest" --become --ask-become-pass

##		Upgrade all the package updates that are available
###			ansible all -m apt -a "upgrade=dist" --become --ask-become-pass

