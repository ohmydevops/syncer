# sync-ssh-keys-with-github
Sync SSH public keys on my github with my server (Automated)

```shell
crontab -e
*/5 * * * * /usr/bin/wget https://github.com/USER_NAME.keys -O /tmp/authorized_keys.tmp && mv /tmp/authorized_keys.tmp /root/.ssh/authorized_keys
```
