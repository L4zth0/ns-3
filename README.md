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
Once the docker build is finished must tag and run the image:
```
sudo docker tag ns3-mptcp <IMAGE_ID>
```
```
docker run ns3-mptcp
```
or to run in terminal 
```
sudo docker run -v /Home/Documents/configuration:/mnt  -it --rm --privileged --pid='host' --network host -v /var/run/docker.sock:/var/run/docker.sock ns3-mptcp /bin/bash
```
On the container, run these comands and you can check the MP-TCP activities you may be asked to run 
```
$ cd /src/mptcp
```
```
CXXFLAGS="-Wall" ./waf configure build 
```
```
./waf --run "mptcp"
```
