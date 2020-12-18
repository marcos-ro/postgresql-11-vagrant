# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "debian/buster64"
  config.vm.hostname = "postgresql"

  config.vm.network "forwarded_port", guest: 5000, host: 5423, protocol: "tcp", host_ip: "127.0.0.1"

  config.vm.provider "virtualbox" do |vb|
     vb.gui = false
     vb.memory = "1024"
     vb.cpus = "1"
  end

  config.vm.provision "ansible_local" do |ansible_local|
    ansible_local.playbook = "provision/playbook.yml"
    ansible_local.verbose = true
  end
end
