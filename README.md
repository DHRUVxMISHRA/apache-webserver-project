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

## Project Structure

apache-webserver-project/

├── config/
│   └── httpd.conf
│
├── scripts/
│   └── install-httpd.sh
│
├── ssl/
│   └── ssl-setup.md
│
├── website/
│   └── index.html
│
└── README.md

## Current Status

✅ Apache Installed

✅ Static Website Hosted

✅ Custom Apache Configuration

✅ Domain Connected

✅ HTTPS Enabled

🔄 Next Phase:

* Custom Error Pages
* Virtual Hosts
* Multiple Website Hosting
* Reverse Proxy
* Load Balancing

## Domain

https://dhruvmishra.co.in
