# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.ssh.insert_key = false
  
    config.vm.define "cassandra1" do |cassandra|
      cassandra.vm.hostname = "cassandra1"
      cassandra.vm.box = "centos/7"
      cassandra.vm.network :private_network, ip: "192.168.0.8"
      cassandra.vm.network :forwarded_port, guest: 22, host: 2208, id: "ssh"
      cassandra.vm.provider "virtualbox" do |vb|
        vb.gui = false
        vb.cpus = 1
        vb.memory = 2048
    end
  end
end