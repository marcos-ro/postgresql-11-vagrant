# -*- mode: ruby -*-
# vi: set ft=ruby :
# Vagrantfile
# Copyright(C) 2021 marcos-ro <marcosroropeza+github@gmail.com>
#
# Distributed under terms of MIT license
#

Vagrant.configure("2") do |config|
  # Config basic
  config.vm.box      = "debian/buster64"
  config.vm.hostname = "postgresql"

  # Config private network for comunicate out of the vagrant box
  config.vm.network "private_network", ip: "192.168.1.101"

  # Config forwarded_port for postgresql listener
  config.vm.network "forwarded_port",
      guest: 5000,
      host: 5000,
      protocol: "tcp",
      host_ip: "192.168.1.101",
      auto_correct: true

  # Config minimal virtualbox
  config.vm.provider "virtualbox" do |vb|
     vb.gui    = false
     vb.memory = "1024"
     vb.cpus   = "1"
  end

  # Config local provision
  config.vm.provision "ansible_local" do |ansible_local|
    ansible_local.playbook = "provision/playbook.yml"
    ansible_local.verbose  = true
  end
end
