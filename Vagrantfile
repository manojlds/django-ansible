# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  
  config.vm.box = "precise32"

  config.vm.network :private_network, ip: "192.168.33.10"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "site.yml"
    ansible.inventory_path = "hosts"
    ansible.verbose = "v"
  end
end
