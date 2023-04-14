Vagas 
# -*- mode: ruby -*-
# vi: set ft=ruby :


# Autor: Aramis de Oliveira


# This configration below create four machines for a cluster K8s at once

Vagrant.configure("2") do |config|
  config.vm.define "Runcher-ubuntu" do |subconfig|
  subconfig.vm.box = "ubuntu/xenial64"
  config.vm.box_check_update = false
  subconfig.vm.network "private_network", ip: "192.168.33.219"
  subconfig.vm.network "public_network", ip: "192.168.0.219"
  subconfig.vm.hostname = "Runcher-ubuntu"


  config.vm.provider "virtualbox" do |vb|
  #Display the VirtualBox GUI when booting the machine
     vb.gui = true
 
  #Customize the amount of memory on the VM:
     vb.memory = "4096"
     vb.cpus = 2
   end
end
  config.vm.define "K8s-1" do |subconfig2|
  subconfig2.vm.box = "ubuntu/xenial64"
  config.vm.box_check_update = false
  subconfig2.vm.network "private_network", ip: "192.168.33.220"
  subconfig2.vm.network "public_network", ip: "192.168.0.220"
  subconfig2.vm.hostname = "K8s-1" 
end
  config.vm.define "K8s-2" do |subconfig3|
  subconfig3.vm.box = "ubuntu/xenial64"
  config.vm.box_check_update = false
  subconfig3.vm.network "private_network", ip: "192.168.33.221"
  subconfig3.vm.network "public_network", ip: "192.168.0.221"
  subconfig3.vm.hostname = "K8s-2" 
end
  config.vm.define "K8s-3" do |subconfig4|
  subconfig4.vm.box = "ubuntu/xenial64"
  config.vm.box_check_update = false
  subconfig4.vm.network "private_network", ip: "192.168.33.222"
  subconfig4.vm.network "public_network", ip: "192.168.0.222"
  subconfig4.vm.hostname = "K8s-3" 
end
  config.vm.define "K8s-4" do |subconfig4|
  subconfig4.vm.box = "ubuntu/xenial64"
  config.vm.box_check_update = false
  subconfig4.vm.network "private_network", ip: "192.168.33.223"
  subconfig4.vm.network "public_network", ip: "192.168.0.223"
  subconfig4.vm.hostname = "K8s-4" 
end
