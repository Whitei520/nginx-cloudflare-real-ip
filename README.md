# nginx-cloudflare-real-ip-aapanel

![Example](https://i.imgur.com/9FEGmr4.png)
### Forked from https://virtubox.github.io/nginx-cloudflare-real-ip/ and edited to support aaPanel https://aapanel.com/.

Configure Nginx to restore Visitors real IP under Cloudflare CDN

## Features

* Get Cloudflare IPv4 + IPv6 list and create nginx configuration to restore visitors real IP in `/www/server/panel/vhost/nginx/cloudflare.conf`

## Requirements

* Nginx built with http_realip_module

You can check if http_realip_module available with :

```bash
nginx -V 2>&1 | grep with-http_realip_module
```

If the previous command return nothing, http_realip_module isn't available

---

## Usage

Setup the script to run daily via the cron panel.
Example below:

![Example](https://i.imgur.com/aGVF2d8.png)
