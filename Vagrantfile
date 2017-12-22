# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"

  config.vm.network "private_network", ip: "10.10.10.10"

  config.vm.network "forwarded_port", guest: 5050, host: 5050
  config.vm.network "forwarded_port", guest: 5051, host: 5051
  config.vm.network "forwarded_port", guest: 8080, host: 8080

  config.vm.provider "virtualbox" do |vb|
    vb.cpus   = 1
    vb.memory = 2048
  end
  
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "provisioning/playbook.yml"
    ansible.verbose  = "vv"
  end
end
