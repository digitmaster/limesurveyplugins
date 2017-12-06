# limesurveyplugins
plugins for limesurvey 

LowercaseAuthLDAP  1.0
# Requirements:
WORKS ONLY IF the two files: 
/application/views/admin/user/editusers.php
/application/views/admin/user/setuserpermissions.php 
are patched for accepting any active plugin containing "AuthLDAP" in name. See commits:
https://github.com/digitmaster/LimeSurvey/commit/ab6dec28208f3c1d925d285b32f55c704b6fa51f
https://github.com/digitmaster/LimeSurvey/commit/800f8fc63484e780d39501340953eba6696281ff
# Description: 
This plugin provides admin creation by fetching the specified username from the LDAP field saved in its settings and importing it with lowercase characters for both username and email 
# Installation:  
copy the folder in the plugin directory and set the proper permissions as you did for the rest of the web folders (e.g.: 755)
# Setup: 
exactly as you do with the native AuthLDAP
# Final step: 
deactivate the AuthLDAP plugin
# NOTE:  
do not worry that after adding the user the confirmation messages might now show you the username and email in lowercase because they will be saved lowercase in the limesurvey users' database 
