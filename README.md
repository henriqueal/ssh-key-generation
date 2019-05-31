# Steps to become a developer more faster

- 1) Turn off the password expiration for user henriqueal:
```bash
# chage -M 99999 henriqueal
```

- 2) It's easier remember name than numbers! Configure your 'hosts' to map hostnames to IP addresses:
```bash
## Open hosts file:
$ sudo gedit /etc/hosts

## Add the follow line:
192.168.0.1 app-hom
```

- 3) Stop typing your password! Generate your public ssh-key and install in remote servers:
```bash
## Generating ssh
$ cd ~/.ssh
$ ssh-keygen

## After generate you should have two files (something.pub something)
$ ls
id_rsa id_rsa.pub 

# Now, we can install it in each server we want. Let's install it in server configured in the first step:
$ ssh-copy-id -i ~/.ssh/id_rsa.pub henriqueal@app-hom
```
