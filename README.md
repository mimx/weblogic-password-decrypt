# weblogic-password-decrypt


$ cd oracle_common/common/bin
$ ./wlst.sh

wls:/offline> domain="/oracle/mw/exmaple/user_projects/domains/oam"

wls:/offline> service = weblogic.security.internal.SerializedSystemIni.getEncryptionService(domain)

wls:/offline> encryption = weblogic.security.internal.encryption.ClearOrEncryptedService(service)

wls:/offline> print "Weblogic server Admin password : %s" %encryption.decrypt("{AES}xxxxxxxxx")

Weblogic server Admin password : password
```
