# Module Federation with Rspack - Proof of Concept

This project demonstrates Module Federation implementation using Rspack as an alternative to Webpack. The architecture consists of two applications: a host application and a remote application that communicate with each other through Module Federation.
 
## 🚀 Features

* Module Federation Implementation

* Rspack as bundler

* Host-Remote applications communication

* Dynamic loading of federated modules
  

## 📋 Prerequisites

* Node.js (version 16 or higher)

* npm (included with Node.js)  

## 🛠️ Project Structure

 ``` bash
module-federation-demo/

├── host/ # Main application (host)

└── remote/ # Secondary application (remote)
 ```
  

## ⚙️ Installation and Setup
  

### Host Application
  
 ``` bash
cd host

npm install

npm start
 ```
  

The host application will be available at `http://localhost:3000`  

### Remote Application  

 ``` bash
cd remote

npm install

npm start
 ``` 

The remote application will be available at `http://localhost:3001`

  

## 🔗 How it Works

1. The remote application exposes modules/components that can be consumed by other applications

2. The host application consumes the modules exposed by the remote application

3. Rspack handles compilation and bundling, providing a faster alternative to Webpack

## 📝 Important Notes  

* Both applications must be running for module federation to work properly

* The remote application should be started before the host application

* Ports 3000 and 3001 must be available for proper project execution

## ⚙️ Troubleshooting

1. Verify both applications are running

2. Ensure required ports are available

3. Clear browser cache

4. Run `npm clean-install` in both projects

  

## 📄 License
This is free and unencumbered software released into the public domain.

  

Anyone is free to copy, modify, publish, use, compile, sell, or distribute this software, either in source code form or as a compiled binary, for any purpose, commercial or non-commercial, and by any means.

  

For more information, please refer to [unlicense.org](https://unlicense.org)

## 🔧 Tech Stack
* React
* Rspack
* Module Federation
* Node.js
* npm