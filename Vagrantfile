# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # Virtual machine properties.
  config.vm.box = "quantal64"
  config.vm.network :forwarded_port, host: 8080, guest: 80

  # Chef provisioning.
  config.vm.provision :chef_solo do |chef|
    chef.add_recipe "nginx"
  end
end
