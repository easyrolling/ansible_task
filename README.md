# Challenge - (2 hours)
Sensu is an open source monitoring application that allows you to monitor any 
number of servers and services. It offers many community written plugins like 
monitoring resources on a server and particular application. Sensu also uses 
RabbitMQ and Redis as back-end. For this task, install Sensu on one server and 
monitor all 3 servers for cpu, disk, and memory. You must use Ansible to install 
and configure Sensu. Make sure you are using RabbitMQ and Redis in docker. 
Also install a dashboard for Sensu to show us the status of all 3 servers/checks.
A popular open-source dashboard for Sensu is Uchiwa, but you are free to use any
solution you find.

# Requirements
* You will receive access to 3 test servers.
* Create a Github repo to store all your code. 
* Use Ansible to update the system, install any dependencies, and 
install/configure Docker on all 3 hosts.
* Redis and RabbitMQ should be running in Docker Containers.
* Sensu and its chosen dashboard need not be containerized
* Dashboard Sensu should run on port 3000
* The final solution should be able to install Sensu, Redis, RabbitMQ, and the
  dashboard of choice all on the same machine or all on seperate machines with
  RabbitMQ and Redis running in Docker containers

# Final Deliverable
At the end of 2 hours, you should be able to present to us a Github repository
with your Ansible source code, as well as a dashboard for Sensu running on port
3000 on the master server.

# Resources
* https://docs.docker.com/install/linux/docker-ce/ubuntu/
* https://hub.docker.com/_/rabbitmq/
* https://hub.docker.com/_/redis/
* https://uchiwa.io/
* https://docs.sensu.io/sensu-core/1.2/

# Servers
Username will be ubuntu for all. Each server runs ubuntu 16.04. SSH key can be
found below. The following ports will be open on theses servers: 22, 6379, 5672,
4567, 3000. These servers will only exist until the end of day.

* sensu-master:  35.173.192.6 
* slave0:        18.207.200.35 
* slave1:        54.198.150.180 
