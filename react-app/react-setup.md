# React Application Setup

## Objective

Create a React application and use it as the backend application for demonstrating Apache HTTPD Reverse Proxy functionality.

## Install Node.js

```bash
sudo yum install -y nodejs
```

Verify installation:

```bash
node -v
npm -v
```

## Create React Application

```bash
npx create-react-app my-app
```

This command creates a new React project named:

```text
my-app
```

## Navigate to Project Directory

```bash
cd my-app
```

## Start React Application

```bash
npm start
```

React starts on:

```text
http://localhost:3000
```

## Verification

Open:

```text
http://localhost:3000
```

The default React application page should appear.

## Integration with Apache Reverse Proxy

Apache HTTPD was configured to forward requests received on Port 80 to the React application running on Port 3000.

Request Flow:

User Browser
↓
Apache HTTPD (Port 80)
↓
React Application (Port 3000)
↓
Response Returned to User

## Key Learning

* Node.js Installation
* NPM Usage
* React Application Setup
* React Development Server
* Apache Reverse Proxy Integration

