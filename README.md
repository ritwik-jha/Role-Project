# Ansible Role Project

On running the ansible playbook, httpd server will be installed and configured on the host group named server and the code file home.php will be copied in the document root of all the nodes in this group.

Further the node in host group named loadbalancer will have the haproxy installed and configured and also the haproxy.cfg created using jinga template will be copied in /etc/haproxy/haproxy.cfg of the nodes. 

This edited config file will automatically add the new nodes in the list of backend servers.

so we will have a complete setup of loadbalancer and backend server which will automatically add new nodes when they come up. 
