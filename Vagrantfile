# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box_check_update = false
  config.vm.box = "ubuntu/xenial64"

  config.vm.network "forwarded_port", guest: 5000, host: 80
  # config.vm.network "public_network"
  config.vm.network "public_network", ip: "192.168.1.225"
  # config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
    vb.name = "sqlserver"
    vb.memory = "2024"
    vb.cpus = 1
  end
  # config.vm.synced_folder ".", "/vagrant_data"

  # config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"
  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y apache2
  # SHELL
end
