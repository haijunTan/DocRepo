## 通过docker源安装dokcer 1.9.1 （ubuntu14.04.2 验证OK）
```
$ sudo apt-get install apt-transport-https
$ sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys     36A1D7869245C8950F966E92D8576A8BA88D21E9
$ sudo bash -c "echo deb https://get.docker.io/ubuntu docker main > /etc/apt/sources.list.d/docker.list"
$ sudo apt-get update
$ sudo apt-get install lxc-docker
```
## 卸载Docker包及其以来不再需要使用下面的命令
```
sudo apt-get autoremove --purge docker-engine
```
## 删除所有的镜像，容器和卷，运行下面的命令
```
rm -rf /var/lib/docker
```
### from：http://blog.csdn.net/qq_22841811/article/details/53447560
