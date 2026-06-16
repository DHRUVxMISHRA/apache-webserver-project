# Apache HTTPD Load Balancing

## Overview

In this phase, Apache HTTPD was configured as a Load Balancer to distribute incoming requests across multiple backend web servers. Instead of sending all traffic to a single server, Apache forwards requests to a cluster of servers, improving scalability and availability.

## Architecture

Client → Apache Load Balancer → Backend Servers

Backend Servers:

* Server-1 (Apache Web Server)
* Server-2 (Apache Web Server)

## Backend Server Configuration

Each backend server was configured with:

* Apache HTTPD installed
* Custom index.html page
* Apache service started and enabled

Example verification:

```bash
http://SERVER-1-IP
```

Output:

```text
This is our Server-1!!!!
```

```bash
http://SERVER-2-IP
```

Output:

```text
This is our Server-2!!!!
```

## Apache Load Balancer Configuration

Configuration file:

```bash
/etc/httpd/conf.d/mywebsite2.conf
```

```apache
<VirtualHost *:80>

    ServerName mywebsite2.com
    ServerAlias www.mywebsite2.com

    <Proxy "balancer://mycluster">

        BalancerMember http://SERVER-1-IP:80
        BalancerMember http://SERVER-2-IP:80

        ProxySet lbmethod=byrequests

    </Proxy>

    ProxyPass "/" "balancer://mycluster/"
    ProxyPassReverse "/" "balancer://mycluster/"

</VirtualHost>
```

## Key Directives

### BalancerMember

Registers backend servers in the load balancing cluster.

### ProxyPass

Forwards incoming requests to the backend cluster.

### ProxyPassReverse

Handles redirects and response headers correctly.

### lbmethod=byrequests

Implements Round Robin request distribution.

## Verification

Reload Apache:

```bash
sudo systemctl reload httpd
```

Test using:

```bash
curl http://LOAD-BALANCER-IP
```

Refresh multiple times to observe responses from different backend servers.

## Benefits

* Improved scalability
* Better resource utilization
* High availability
* Fault tolerance
* Simplified traffic management

## Learning Outcomes

* Apache HTTPD Load Balancing
* Backend Server Clustering
* ProxyPass and ProxyPassReverse
* Round Robin Load Distribution
* Traffic Distribution Across Multiple Servers
* Basic High Availability Concepts

