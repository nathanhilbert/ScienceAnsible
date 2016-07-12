# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.define "trusty" do |trusty|
    trusty.vm.box = "ubuntu/trusty64"
  end 

  # config.vm.network "private_network", ip: "192.168.99.151",
  #   virtualbox__intnet: true
  config.vm.hostname = "urbis"

  config.vm.provision "ansible" do |ansible|
      ansible.playbook = "main.yml"
  end

  config.vm.synced_folder "data/homeshare", "/home/vagrant/homeshare", owner: "vagrant", group: "vagrant"

  config.vm.provider "virtualbox" do |v|
    config.vm.network "private_network", ip: "192.168.99.152", :name => 'vboxnet0', :adapter => 2
    v.memory = 3096 # sfcgal compilation needs a minimum of 3GB
    v.cpus = "2"
  end
end
