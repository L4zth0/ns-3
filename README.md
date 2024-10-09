# Multipath -TCP in NS-3 on Docker
build the environment MPTCP  on docker.

## How to use
First install docker-compose 
```
sudo apt-get install docker-compose
```

### Download the Dockerfile and run

After downloading and extracting the zip file, enter the folder and run :
```
docker-compose up -d
```
or the next command:

```
docker build - < Dockerfile
```
On the container, run these comands and you can check the MP-TCP activities you may be asked to run ```./waf configure```
```
$ cd /src/mptcp
$./waf --run "mptcp"
```
