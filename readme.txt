praticing ansible

Really just notes and such for myself.

Trying to figure out how to work with docker containers with a non-docker host. All containers state they have an OS that is the same as the control node and pretty sure that is not true.
Getting the OS via bash in the containers:
The MSSQL container is Ubuntu 20.4
The Apache container is Apache 2.4.48 (Unix).
For the apache the playbook states it is a Ubuntu 20.4

Got it to work, had to allow Docker to intergrate with the wsl ubuntu distro. Also updated the hostDocker file to help fix some problems.
The name of the host needs to be same as the docker container. 

Debian does not support LSB, however, instead of failing it just returns an empty array. 

Stopping a container will make it unreachable as expected. 
