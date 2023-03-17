# Creez une image Almalinux avec supervisord et sshd
```shell
docker build -t puppet-agent-almalinux .   # build the image
docker run -d --name alma --add-host puppet:<puppetmaster_ip> puppet-agent-almalinux  # container alma created
docker ps # check 
docker logs alma # see container logs
# sshd and puppet agent  must have pid 
```