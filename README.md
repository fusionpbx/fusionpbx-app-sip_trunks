# SIP Trunks
Basic application to create bridge statements for registered endpoints. The SIP trunks are used for inbound calls. It removes the extension from the contact string and passes the original number that was called. This is useful for a PBX that is registered to the extension.
When using an ATA FXO, this may not matter if you don't need the extension number removed; in that case, you can skip the SIP Trunks feature and send calls direct to the extension

Install
```
cd /var/www/fusionpbx/app
git clone https://github.com/fusionpbx/fusionpbx-app-sip_trunks.git sip_trunks
php /var/www/fusionpbx/core/upgrade/upgrade.php
php /var/www/fusionpbx/core/upgrade/upgrade.php --permissions
```

Permission
- sip_trunk_destinations
  - superadmin
  - admin

This will be accessible in the Destination Select list under Category SIP Trunks. You will see one for every extension.
