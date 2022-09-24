# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.network "forwarded_port", guest: 80, host: 8888

  config.vm.define "server_centos" do |server_centos|
    server_centos.vm.box = "bento/centos-7.9"
    server_centos.vm.hostname = "server-centos"
    server_centos.vm.synced_folder "./ansible","/home/vagrant/ansible"
    server_centos.vm.provision "shell", inline: <<-SHELL
      sudo yum install epel-release -y
      sudo yum install ansible -y
    SHELL
  end
end
