# Vagrantfile
# vim: set ft=ruby ts=2 :

Vagrant.configure("2") do |config|
  config.vm.box = "k8s"
  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 2
  end

  config.vm.define :master do |cfg|
    cfg.vm.hostname = "master"
    cfg.vm.network :public_network, ip: "192.168.10.90"
  end

  config.vm.define :node1 do |cfg|
    cfg.vm.hostname = "node1"
    cfg.vm.network :public_network, ip: "192.168.10.91"
  end

  config.vm.define :node2 do |cfg|
    cfg.vm.hostname = "node2"
    cfg.vm.network :public_network, ip: "192.168.10.92"
  end

  config.vm.synced_folder "./", "/vagrant"
end