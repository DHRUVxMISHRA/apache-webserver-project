# Multiple Website Hosting using Apache Virtual Hosts

## Objective

Host multiple websites on a single Apache server using Virtual Hosts.

## Website 1

Domain:
dhruvmishra.co.in

Document Root:
/var/www/dhruvmishra.co.in

Port:
443

## Website 2

Domain:
mywebsite2.com

Document Root:
/var/www/mywebsite2

Port:
80

## Virtual Host Configuration

ServerName:
mywebsite2.com

ServerAlias:
www.website2.com

Dedicated Logs:
mywebsite2_error.log
mywebsite2_access.log

## Benefits

- Multiple websites on one server
- Reduced infrastructure cost
- Separate document roots
- Separate logs
- Easier management

## Commands Used

sudo httpd -t

sudo systemctl reload httpd

sudo systemctl status httpd
