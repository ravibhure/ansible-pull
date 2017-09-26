# ansible-pull
test ansible-pull

[ansible-pull](https://linux.die.net/man/1/ansible-pull) - set up a remote copy of ansible on each managed node

* Example: `ansible-pull -U <url>`

```
ravi@ubuntu:~$ ansible-pull -U https://github.com/ravibhure/ansible-pull
Starting Ansible Pull at 2017-09-26 10:32:29
/usr/local/bin/ansible-pull -U https://github.com/ravibhure/ansible-pull
localhost | SUCCESS => {
    "after": "4bc011a2c5c9ed04298296206c22d7b955b275f4",
    "before": null,
    "changed": true
}
 [WARNING]: Found both group and host with same name: localhost

PLAY [testlocal] ************************************************************************************************************************

TASK [debug] ****************************************************************************************************************************
ok: [localhost] => {
    "msg": "echo hello"
}

PLAY RECAP ******************************************************************************************************************************
localhost                  : ok=1    changed=0    unreachable=0    failed=0

```
