# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "quantal64"
  config.vm.network :forwarded_port, host: 8080, guest: 80

Vagrant.configure("2") do |config|
  chef.add_recipe "nginx"
end

end
