# ThingML Editor embedded on docker

[Docker hub](https://hub.docker.com/r/madkira/thingmleditor/)
[Thingml repository](https://github.com/TelluIoT/ThingML)

## &#x1F537; Purpose

Have an easy deployment environment in order to install and use ThingML throught docker.

## &#x1F537; Installation
#### by cloning
```
git clone https://github.com/madkira/thingmleditor.git
cd thingmleditor
./build
```
#### throught docker hub
```
mkdir thingml
docker pull madkira/thingmleditor
```

## &#x1F537; Run
make sure that you have environment variable DISPLAY defined and to have the right access
```
xhost +si:localuser:$USER
```
#### with the script
```
cd [path_where_you_clone]/thingmleditor
./eclipse
```
#### directly with the commandline
```
docker run -ti --rm -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix -v [path_where_you_clone]/thingml:/home/developer -v [path_where_you_clone]:/workspace madkira/thingmleditor
```

## &#x1F537; More

**Visit [thingml.org](http://www.thingml.org) to find out more about ThingML !**


![ThingML is released under OSI-compliant Apache 2.0 license](https://opensource.org/files/osi_keyhole_100X100_90ppi.png "ThingML is released under OSI-compliant Apache 2.0 license")
