# Multipath -TCP in NS-3 on Docker
build the environment MPTCP  on docker.

## How to use

Download the Dockerfile and run 
```
docker-compose up -d
```
On the container, run these comands and you can check the MP-TCP activities you may be asked to run ```./waf configure```
```
$ cd /src/mptcp
$./waf --run "mptcp"
```
