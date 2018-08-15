# Project Title

Keyflow-Website Standalone Server

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Prerequisites
```
Node 
Npm
Dockers
```
### How to run and test keyflow-website on your local machine
- Install node,npm and dockers. 
- Clone keyflow-website repository into your local machine.
- Run npm install, after that to auto update code changes to server you need to open a terminal in the project directory and run `make watch`. 
- If you see an error after running `make watch` follow these steps to remove the error.
```
Go to node_modules and search for parallelshell module.
Open parallelshell folder and then open index.js.
On line `105` you will see this code -> `cwd: process.cwd`.
Replace that code with `cwd: process.cwd()` and it will start working.
```
After that run your dockers server and open a terminal in project directory and run the following command:
```
sh run_docker_server.sh
```
It will start your server. Wait until you see this message on your terminal 
```
`KEYFLOW WEBSITE OPTIONS "0"`
```
You can now check it on 

```stage-www.localhost:5000/en/cities```
