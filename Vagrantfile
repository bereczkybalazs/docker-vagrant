# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
    config.vm.define "dev-machine" do |docking|
        docking.vm.box = "williamyeh/ubuntu-trusty64-docker"
        config.vm.network "forwarded_port", guest: 80, host: 3222, host_ip: "127.0.0.1"
        config.vm.network "private_network", ip: "192.168.33.10"
    end
    config.vm.synced_folder "./","/home/vagrant"
end
