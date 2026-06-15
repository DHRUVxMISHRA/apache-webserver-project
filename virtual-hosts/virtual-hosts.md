# Apache Virtual Hosts

## Objective

Configure Apache Virtual Hosts to host websites using separate configuration files and dedicated document roots.

## Changes Made

### Apache Main Configuration

Added:

IncludeOptional conf.d/*.conf

This allows Apache to automatically load all configuration files stored inside:

/etc/httpd/conf.d/

### Virtual Host Configuration

Created:

/etc/httpd/conf.d/dhruvmishra.co.in.conf

### Dedicated Website Directory

Created:

/var/www/dhruvmishra.co.in

Moved website files:

* index.html
* styles.css
* error_404.html

from:

/var/www/html

to:

/var/www/dhruvmishra.co.in

## Virtual Host Configuration

The virtual host serves:

dhruvmishra.co.in

using HTTPS on port 443.

Document Root:

/var/www/dhruvmishra.co.in

SSL Certificate:

Let's Encrypt

Custom Error Page:

error_404.html

## Verification

Validate configuration:

sudo httpd -t

Restart Apache:

sudo systemctl restart httpd

Check service:

sudo systemctl status httpd

## Outcome

Apache now uses a dedicated Virtual Host configuration and document root for the website, enabling future support for hosting multiple domains on the same server.

