# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "ttree/workshop-neos"

  config.vm.synced_folder ".", "/vagrant", type: "nfs"

  config.vbguest.auto_update = false

  config.ssh.forward_agent = true

  config.vm.network "private_network", ip: "192.168.77.21"
  config.vm.hostname = 'www.neos-workshop.box'

  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 2
  end

end
