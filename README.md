# Apache Web Server Project

## Overview
This project demonstrates the complete setup and configuration of Apache HTTPD on AWS EC2 (Amazon Linux 2023), including custom website hosting, domain configuration, and HTTPS security using Let's Encrypt SSL certificates.

## Tech Stack

* AWS EC2
* Amazon Linux 2023
* Apache HTTPD
* Let's Encrypt
* Certbot
* DNS Configuration
* SSL/TLS

## Project Architecture

User → Domain → AWS EC2 → Apache HTTPD → Virtual Hosts → Multiple Websites

## Features Implemented

### Phase 1: Apache Installation

* Installed Apache HTTPD
* Started and enabled Apache service
* Verified web server accessibility

### Phase 2: Static Website Hosting

* Created custom index.html
* Hosted website using Apache DocumentRoot
* Verified browser access

### Phase 3: Custom Apache Configuration

* Created minimal Apache configuration
* Configured ServerRoot
* Configured DocumentRoot
* Configured DirectoryIndex
* Configured Error Logging

### Phase 4: Custom Domain Setup

* Purchased domain: dhruvmishra.co.in
* Configured DNS A Record
* Connected domain to EC2

### Phase 5: HTTPS & SSL

* Installed Certbot
* Generated Let's Encrypt SSL Certificate
* Configured Apache for HTTPS
* Enabled Port 443
* Secured website using SSL/TLS

### Phase 6: Custom Error Pages

* Created custom 404 error page
* Configured Apache ErrorDocument directive
* Improved user experience for invalid URLs
* Reloaded Apache configuration

### Phase 7: Apache Virtual Hosts

* Created dedicated website document root
* Configured Apache Virtual Host
* Enabled configuration loading from conf.d
* Moved website-specific settings from httpd.conf
* Prepared server for hosting multiple websites

### Phase 8: Multiple Website Hosting

* Hosted multiple websites on a single Apache server
* Created separate Virtual Host configuration
* Configured ServerName and ServerAlias
* Configured dedicated log files
* Implemented multi-site architecture

## Project Structure

```text
apache-webserver-project/
├── README.md
├── configs/
│   └── httpd.conf
├── domain/
│   └── domain-setup.md
├── error-pages/
│   ├── error-pages.md
│   └── error_404.html
├── scripts/
│   └── install-httpd.sh
├── ssl/
│   ├── changes.md
│   └── ssl-setup.md
├── virtual-hosts/
│   ├── dhruvmishra.co.in.conf
│   └── virtual-hosts.md
├── multi-site-hosting/
│   ├── mywebsite2.conf
│   └── multi-site-hosting.md
└── website/
    └── styles.css
```

## Important Files

### Apache Configuration

- `configs/httpd.conf` → Main Apache configuration

### Website Files

- `website/index.html` → Homepage
- `website/styles.css` → Website styling

### Error Handling

- `error-pages/error_404.html` → Custom 404 page
- `error-pages/error-pages.md` → Error page documentation

### Domain Configuration

- `domain/domain-setup.md` → Domain and DNS setup notes

### SSL Configuration

- `ssl/ssl-setup.md` → SSL/TLS setup
- `ssl/changes.md` → SSL configuration changes

### Virtual Hosts

- `virtual-hosts/dhruvmishra.co.in.conf` → Primary website Virtual Host
- `virtual-hosts/virtual-hosts.md` → Virtual Host notes

### Multi-Site Hosting

- `multi-site-hosting/mywebsite2.conf` → Second website configuration
- `multi-site-hosting/multi-site-hosting.md` → Multi-site hosting notes

### Automation

- `scripts/install-httpd.sh` → Apache installation script| install-httpd.sh | Apache installation script |

## Current Status

✅ Apache Installed

✅ Static Website Hosted

✅ Custom Apache Configuration

✅ Domain Connected

✅ HTTPS Enabled

✅ Custom Error Pages

🔄 Next Phase:

* Reverse Proxy
* Load Balancing
* Load Balancing

## Domain

https://dhruvmishra.co.in

## Learning Outcomes

Through this project I learned:

* Apache HTTPD Installation and Configuration
* Linux File and Service Management
* AWS EC2 Administration
* DNS Configuration
* Domain Mapping
* SSL/TLS Concepts
* Let's Encrypt and Certbot
* Custom Error Page Handling
* Web Server Troubleshooting
* Apache Virtual Hosts
* Multi-Site Hosting Architecture
* Domain-Based Website Routing
* Apache Multi-Site Hosting
* ServerName and ServerAlias Configuration
* Dedicated Website Logging
* Dedicated Website Logging
* Name-Based Virtual Hosting
