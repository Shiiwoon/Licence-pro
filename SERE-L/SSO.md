# Authentification Unique - Single Sign On

> Config : Debian 8
***
## Mise en place d'un authentification KERBEROS depuis un annuaire LDAP

---
#### Installation OpenLDAP

> Interroger la base de données des paquets pour obtenir les informations demandées / **Non Obligatoire**
         
         # aptitude search '?description(OpenLDAP)'
         
![alt text](http://nsa38.casimages.com/img/2017/03/06/170306030131739250.png "SSO1")
```debian
    # aptitude install slapd ldap-utils
```

> Identifier le processus

        # ps aux | grep l[d]ap

> Identifier les ou les n° de ports ouverts par le OpenLDAP 389

    # grep ldap /etc/services
    # netstat -nat