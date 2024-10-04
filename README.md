This is an example of a [Catapult](https://github.com/ClarifiedSecurity/catapult) project which installs a dockerized Sonatype Nexus onto a target machine using Nginx as its proxy. 

To run this on your preferred target you need to change 3 parameters in `host_vars/proovikas.yml`:
`connection_address:` target IP address here  
`ansible_deployer_username:` target's username here (with root access)  
`ansible_deployer_password:` target user's password here  


Run with:
`ctp host deploy proovikas`

You should see the GUI of Nexus if you open a browser on the target machine and navigate to `proovikas.example.com`
