### problem 1
```
start.sh: line 1: ./binaries/service-avx2: Permission denied
```
### solve
sudo chmod -R 777 rtm
### problem 2
```
could not select device driver "" with capabilities: [[gpu]]
```
### solve
```
sudo apt install -y nvidia-docker2
sudo systemctl daemon-reload
sudo systemctl restart docker
```
### problem 3
error while loading shared libraries: libssl.so.1.1
### slove
[cryptoprofi](https://www.cryptoprofi.info/?p=8678)
