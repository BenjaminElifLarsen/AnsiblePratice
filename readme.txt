praticing ansible

Trying to figure out how to work with docker containers with a non-docker host. All containers state they have an OS that is the same as the control node and pretty sure that is not true.
Getting the OS via bash in the containers:
The MSSQL container is Ubuntu 20.4
The Apache container is Apache 2.4.48 (Unix).
For the apache the playbook states it is a Ubuntu 20.4