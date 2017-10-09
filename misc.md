# MISC

## Generate a SSH key on a remote server and copy to local clipboard

```bash
# remote
ssh-keygen -t rsa -b 4096 -C "lawrencefeipan@gmail.com"
# local
scp root@123.123.213.123:/root/.ssh/id_rsa.pub /tmp
xclip -sel clip < /tmp/id_rsa.pub
```
