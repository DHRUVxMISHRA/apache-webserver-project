# Apache Reverse Proxy

## Objective

Configure Apache HTTPD as a Reverse Proxy for a React application running on port 3000.

## Backend Application

Technology:
React

Port:
3000

Address:
http://127.0.0.1:3000

## Apache Reverse Proxy Configuration

ProxyPreserveHost On

ProxyPass / http://127.0.0.1:3000/

ProxyPassReverse / http://127.0.0.1:3000/

## Benefits

- Hide backend application
- Centralized access point
- Better security
- SSL termination support
- Load balancing support
- URL routing

## Verification

sudo httpd -t

sudo systemctl reload httpd

## Architecture

User
 ↓
Apache HTTPD
 ↓
React Application
(Port 3000)
