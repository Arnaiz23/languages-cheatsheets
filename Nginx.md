# Nginx cheatsheet

## Directory

`/etc/nginx`

## Structure

Path | Purpose
--- | ---
conf.d | Extra configuration files
nginx.conf | The primary configuration files
modules-available | All the modules availables
modules-enabled | All the modules modules-enabled
sites-available | Extra virtual host configuration files
sites-enabled | Symlink to sites-available/<file> to enable vhost


## Logs

- /var/log/nginx/access.log
- /var/log/nginx/error.log


## Check syntax

`nginx -t`

## Nginx SPA

```bash
location / {
	try_files $uri $uri/ /index.html
}
```
