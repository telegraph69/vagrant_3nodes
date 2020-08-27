# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "centos/7"

  (1..3).each do |i|
    config.vm.define "node0#{i}" do |node|
      config.vm.provider "hyperv" do |vb|

        vb.memory = "1024"  
        vb.cpus = "2"
      end
      node.vm.hostname = "node0#{i}"
    end
  end

end