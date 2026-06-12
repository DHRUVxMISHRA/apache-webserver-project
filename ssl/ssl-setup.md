SSL/TLS Setup using Let's Encrypt

Domain:
dhruvmishra.co.in

Server:
Amazon Linux 2023 EC2

Commands Used:

sudo systemctl stop httpd

sudo yum install certbot python3-certbot-apache -y

sudo certbot certonly --standalone -d dhruvmishra.co.in

sudo httpd -t

sudo systemctl start httpd

Certificate Location:
/etc/letsencrypt/live/dhruvmishra.co.in/fullchain.pem

Private Key:
/etc/letsencrypt/live/dhruvmishra.co.in/privkey.pem

Port Opened:
443 (HTTPS)

Outcome:
Website successfully secured with HTTPS.
