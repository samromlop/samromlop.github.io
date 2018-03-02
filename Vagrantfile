# -*- mode: ruby -*-
 
# vi: set ft=ruby :
 
hosts = {
 
  "servidor1" => "192.168.1.101",
  
}
 
Vagrant.configure("2") do |config|
 
  config.vm.box = "debian/stretch64"
 
 hosts.each do |name, ip|
 
    config.vm.define name do |machine|
 
      machine.vm.network :private_network, ip: ip
 
      machine.vm.provider "virtualbox" do |v|
 
        v.name = name
 
      end
 
    end
 
  end
 
end

