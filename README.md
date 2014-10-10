# update Bash on Debian / Ubuntu and RedHat

I copied this code from https://raymii.org/s/articles/Patch_CVE-2014-6271_Shellshock_with_Ansible.html
Thanks to Remy van Elst for writing this code.

I wanted to learn Ansible for a while now and want to and this example was really helpful.

If you want to make this work for your servers, you'll need to have a an [Ansible Inventory File](http://docs.ansible.com/intro_inventory.html).


### how to use

`$ ansible-playbook --limit=<hosts> playbooks/update.yml -K`

Options:

- `  -K, --ask-sudo-pass   ask for sudo password` 
- `  -v, --verbose         verbose mode (-vvv for more, -vvvv to enable connection debugging)`


#### hosts available ?
`$ ansible <hosts> -m ping`

#### what is deployed ?
`$ ansible <hosts> -m setup`
