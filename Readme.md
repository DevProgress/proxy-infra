Tools for managing the VPS portion of the Ad Proxy network.

The primary tool is Ansible, which fits well since our only server-side 

Install on an Ubuntu system that needs a private key and sudo access to add a new user:

`$ ansible-playbook -u ubuntu setupProxy.yml --private-key ~/.ssh/YOUR-PRIVATE-KEY -i 54.80.36.232, --become --become-user=root`

Note: The comma after the IP address is intentional and necessary.

