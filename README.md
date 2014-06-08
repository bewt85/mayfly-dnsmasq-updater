mayfly-dnsmasq-updater
======================

This is part of [mayfly](https://github.com/bewt85/mayfly) which demonstrates the 
concept of testing groups of versions of services in short lived virtual environments.

This is a docker container which mounts the volumes from a [dnsmasq](https://github.com/bewt85/docker-dnsmasq) 
container.  It is used to run scripts which update the mounted `/etc/dnsmasq/hosts` 
file accordingly.

You can build your own versions of this container by setting the following environment variable 
to your docker index username (if you don't it uses mine) and running this bash script:

```
export DOCKER_ACCOUNT_NAME=<your_name>
sudo -E ./build.sh
```
