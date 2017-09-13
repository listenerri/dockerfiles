> based on centos:6.9
> use a script from [wdlinux.cn](http://wdlinux.cn) to install Apache,Mysql,PHP 
> you can take a look at [http://wdlinux.cn/lanmp/install.html](http://wdlinux.cn/lanmp/install.html) for detail

# HOW TO

## build a image
``` shell
# build a image which is named "lamp" with tag "centos6.9"

docker build -t lamp:centos6.9 .
```
## create and run container
``` shell
# create and run a container which is named lamp-centos6.9
# bind host's port 80 and 8080 to container's
# map host's /php/project/directory to container's /www/web
# NOTE! without -it the container will exit immediately!

docker run --name lamp-centos6.9 -p 80:80 -p 8080:8080 -v /php/project/directory:/www/web -it -d lamp:centos6.9
```
## start a container
```
# start a container by name
docker start lamp-centos6.9
```
