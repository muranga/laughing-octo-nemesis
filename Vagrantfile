# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "precise64"
  config.vm.network :forwarded_port, host: 4567, guest: 80
  
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "provision/playbook.yml"
  end    
    
end
