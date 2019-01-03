## Magento
The infrastructure is now installed, but the environment may still be installing the Magento eCommerce itself. This may take up to 30 minutes still.

### Credentials
* **Admin panel URL:** ${env.protocol}://${settings.magento_domain}/admin/ 
* **Secondary URL:** ${env.protocol}://${env.domain}/admin/ 
* **Username:** ${globals.MAGENTO_ADMIN_USERNAME} 
* **Password :** ${globals.MAGENTO_ADMIN_PASSWORD} 

### Domain
If you used custom domain name for the Magento you need to set the public IP address from the Hitch node to the DNS records for that domain. 
  
## PHPMyAdmin
PHPMyAdmin is installed with the database cluster master node. 
* **Admin panel URL:** https://node${nodes.sqldb.master.id}-${env.domain} 
* **Username:** ${globals.MYSQL_ROOT_USERNAME} 
* **Password:** ${globals.MYSQL_ROOT_PASSWORD}

