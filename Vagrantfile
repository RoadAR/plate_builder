# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "alt6"
  config.ssh.sudo_command = "sudo -H %c"
  config.vm.synced_folder ".", "/vagrant"

  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 4
  end
end
