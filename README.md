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

User → Domain → AWS EC2 → Apache HTTPD → Static Website

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
└── website/
    ├── index.html
    └── styles.css
```

## Important Files

| File | Purpose |
|--------|---------|
| httpd.conf | Apache main configuration |
| index.html | Main website page |
| styles.css | Website styling |
| error_404.html | Custom 404 error page |
| ssl-setup.md | SSL configuration notes |
| domain-setup.md | Domain configuration notes |
| install-httpd.sh | Apache installation script |

## Current Status

✅ Apache Installed

✅ Static Website Hosted

✅ Custom Apache Configuration

✅ Domain Connected

✅ HTTPS Enabled

✅ Custom Error Pages

🔄 Next Phase:

* Virtual Hosts
* Multiple Website Hosting
* Reverse Proxy
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
