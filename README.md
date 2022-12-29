# Syncer
Sync SSH public keys on my GitHub with my server (Every 5 minutes)

```shell
➜  ~ crontab -e
➜  ~ */5 * * * * /usr/bin/wget https://github.com/USER_NAME.keys -O /tmp/authorized_keys.tmp && \
            mv /tmp/authorized_keys.tmp /root/.ssh/authorized_keys && echo "Done"
```
