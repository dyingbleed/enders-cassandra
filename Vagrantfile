# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.ssh.insert_key = false

  config.vm.define "cassandra1" do |cassandra|
    cassandra.vm.hostname = "cassandra1"
    cassandra.vm.box = "centos/7"
    cassandra.vm.network :private_network, ip: "192.168.0.10"
    cassandra.vm.network :forwarded_port, guest: 22, host: 2210, id: "ssh"
    cassandra.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.memory = 2048
    end
  end

  config.vm.define "cassandra2" do |cassandra|
    cassandra.vm.hostname = "cassandra2"
    cassandra.vm.box = "centos/7"
    cassandra.vm.network :private_network, ip: "192.168.0.11"
    cassandra.vm.network :forwarded_port, guest: 22, host: 2211, id: "ssh"
    cassandra.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.memory = 2048
    end
  end

  config.vm.define "cassandra3" do |cassandra|
    cassandra.vm.hostname = "cassandra3"
    cassandra.vm.box = "centos/7"
    cassandra.vm.network :private_network, ip: "192.168.0.12"
    cassandra.vm.network :forwarded_port, guest: 22, host: 2212, id: "ssh"
    cassandra.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.memory = 2048
    end
  end
end