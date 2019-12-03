# Utility files for juju
- mostly used for ease of local development
- both should be placed in $PATH such that JUJU can read and use them (juju dynamically searches the path for files prefixed with `juju`)
## Juju-db
- mostly used to connect to the underlying database per cli
- echos important information like IP, name, user, pass
- which can be used to connect with a mongodb client like compass https://www.mongodb.com/products/compass
### Usage
```
machine 0
ip "10.75.147.162"
user: machine-0
pass: somepass

MongoDB shell version v3.6.3
connecting to: mongodb://127.0.0.1:37017/juju
2019-12-03T13:20:25.662+0000 W NETWO
```

## juju-debug
- mostly used to cp compiled dlv into ubuntu juju machine agent
- shows ip and port to connect to 
### Usage
```
❯ juju debug                         
Using dlv=/home/nam/golang/bin/dlv
model controller
machine 0
agent machine-0
ip "10.75.147.162"
Connecting to process 281
API server listening at: [::]:2345
```
