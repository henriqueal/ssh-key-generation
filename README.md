# Steps to become a developer more faster

- 1) Turn off the password expiration for user henriqueal:
```bash
# chage -M 99999 henriqueal
```

- 2) Configure your 'hosts' to map hostnames to IP addresses:
```bash
## Open hosts file:
$ sudo gedit /etc/hosts

## Add the follow line:
192.168.0.1 plataform-project-environment
192.168.0.2 ocs-gerencia-hom
192.168.0.3 ocs-gerencia-prd
```
