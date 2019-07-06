# catalog-deploy

# Stack: Apache2, PostgreSQL, Lightsail
# IP address and SSH port
http://34.217.27.103
Port: 2200
#Install and Configuration
add user grader  
ssh-keygen sets up for grader  
firewall ports allow: 80 http,  123UDP,  2200TCP  
modfied ~/.ssh permission  
Install fail2ban, sendmail  
Modify apache conf: sites-available/catalog.conf  
Modify __init__.py, catalog.wsgi, catalog.wsgi, database_setup.py, data.py  
Install venv inside /var/www/catalog/catalog/

## project folder:
/var/www/catalog/catalog/
## wsgi entry point:  
/var/www/catalog/catalog.wsgi

# To login as grader
ssh -i ~/path to private key grader@34.217.27.103 -p 2200
