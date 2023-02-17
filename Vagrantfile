# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  config.vm.box = "mrvantage/centos7-minikube"
  config.vm.network "public_network", bridge: "Wi-Fi (AirPort)"
  config.vm.synced_folder "../../Vagrant/minikube", "/vagrant_data"

    config.vm.provider "virtualbox" do |vb|
     vb.gui = false
     vb.cpus = "2" 
     vb.memory = "8192"
   end
  
  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y apache2
  # SHELL
end
