# Introduction
WIP repo using opencv, flask and ngrok with python to stream feeds
of RTSP based cameras with future implementation of GUI in the works.

> :warning: *This repo is forked from [here](https://github.com/DiscoverCCRI/ip_cam) and serves
as a "new version" also developed by [me](https://github.com/akielaries), building off of the application
used for the DiscoverCCRI research study. This project will be open source and welcomes contributors.*

Note: Will also be working on some implementations in C++. For now see some examples on providing basic feed.

**For GTK GUI features**

# Build this project
---
**with Docker**
```
$ git clone git@github.com:DiscoverCCRI/ip_cam.git &&
cd /scripts 
$ docker build -t ip_cam . &&
docker image ls
$ docker container run --privledged -d ip_cam
```
**manually**
```
$ git clone git@github.com:DiscoverCCRI/ip_cam.git &&
cd ip_cam/src &&
python3 test_stream_v1.py proxy_stream.py
```
Enter the IP address of the machine you are hosting this project from in a browser
and your feed should be present. 

# Issues
---

# Examples
---

# Ideas
- think of different py libs to implement GUI, PyQt, Tkinter, etc
- maybe implement my own, if going for speed and effeciency lets write it in C!
- modularize what ever the final result is for the demo into something usable
for an application. 
- if we are using C, research how to a C-based GUI can talk with our existing python
implementations.
- research using GTK with C
- Research using curses (terminal-based GUI)
