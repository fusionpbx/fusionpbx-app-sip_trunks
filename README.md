# fusionpbx-app-sip_trunks
Basic application to create bridge statements for registered endpoints.

Install
```
cd /var/www/fusionpbx/app
git clone https://github.com/fusionpbx/fusionpbx-app-sip_trunks.git sip_trunks
php /var/www/fusionpbx/core/upgrade/upgrade.php
php /var/www/fusionpbx/core/upgrade/upgrade.php --permissions
```

Permission
- sip_trunk_destinations

This will be accessible in the Destination Select list under Category SIP Trunks. You will see one for every extension.
