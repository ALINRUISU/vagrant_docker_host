# -*- mode: ruby -*-
# vi: set ft=ruby :
 
Vagrant.configure("2") do |config|
    config.vm.box = "centos/7"
 
    config.vm.define :docker do |docker_config|
        docker_config.vm.hostname = 'docker'
        docker_config.vm.network "public_network", ip: "192.168.0.17"
    end
 
    config.vm.provider :virtualbox do |virtualbox_config|
        virtualbox_config.name = "docker - Centos 7 Latest"
    end
 
    config.vm.provision :shell, path: "bootstrap.sh"
    
end