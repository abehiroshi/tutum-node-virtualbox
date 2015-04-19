# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.provider :virtualbox do |provider, override|
    override.vm.box = "tutum/node"
    override.vm.network :forwarded_port, guest: 2375, host: ENV['PORT']
    override.vm.synced_folder "./", "/vagrant", disabled: true

    override.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end

end
