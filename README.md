
# Ubuntu Nginx Doc



### File upload size limit - nginx:

- Locate the Nginx configuration file and edit

```bash
  cd /etc/nginx
```
```bash
  nano nginx.conf
```

- After opening nginx.conf file find http block code, add the code below

```bash
  http {
    # add this code in http block
    client_max_body_size 100M;
    ...
  }
```
- Now restart the Nginx
  
```bash
  systemctl restart nginx
```
