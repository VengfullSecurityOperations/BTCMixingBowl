Using Nagios Core
 

Create nagiosadmin User Account

 

You’ll first need to create an Apache user account to be able to log into Nagios.

 

The following command will create a user account called nagiosadmin and you will be prompted to provide a password for the account.

sudo htpasswd -c /usr/local/nagios/etc/htpasswd.users nagiosadmin
When adding additional users in the future, you need to remove -c from the above command otherwise it will replace the existing nagiosadmin user (and any other users you may have added).

 

The login URL for Nagios is:

 

http://serversprivateIP/nagios

or

http://serverspublicIP/nagios

 

For example – http://10.25.5.143/nagios or you can use the servers DNS name

 