# MSSQL Server Docker Container
> Running in a _Ubuntu Xenial 16.04 x64_ Vagrant box with **2 GB RAM** and **1 core**.

## How to use

* `$ vagrant resume`
* `$ vagrant suspend`

The db is running in the port 80 of the box, so you can send request by the URI `localhost` or `192.168.1.225`

### TODO

* Create a script that the box will run in the first boot.
* Install Docker and downdload the mssql image.
* Create a scrip/command that execute the script that runs the container.
