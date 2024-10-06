This is an example of a [Catapult](https://github.com/ClarifiedSecurity/catapult) project which installs a dockerized Sonatype Nexus onto a target `Ubuntu` machine using Nginx as its proxy. 

To run this you need to change 3 parameters in `host_vars/proovikas.yml`:
`connection_address:` target IP address here  
`ansible_deployer_username:` target's username here (with root access)  
`ansible_deployer_password:` target user's password here  


Run with:
`ctp host deploy proovikas`

You should see the GUI of Nexus if you open a browser on the target machine or your own host machine when you navigate to `proovikas.example.com`

Bonus example:

You can disable UAC on a target Win11 machine.
To run this you need to change 3 parameters in `host_vars/windows.yml`:
`connection_address:` target IP address here  
`ansible_deployer_username:` target's username here (with admin permissions)  
`ansible_deployer_password:` target user's password here

Run with:
`ctp host deploy windows`