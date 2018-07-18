Vagrant.configure("2") do |config|
  #  config.vm.box = "hashicorp/precise64"
  #  config.vm.network "private_network", ip: "10.10.0.1", virtualbox__intenet: true
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 2
    end

     # machine1
    config.vm.define "web" do |web|
      web.vm.box = "hashicorp/precise64"
      web.vm.network "private_network", ip: "10.10.0.1"
    end
    config.vm.define "db" do |mysql|
      mysql.vm.box = "hashicorp/precise64"
      mysql.vm.network "private_network", ip: "10.10.0.2"
    end
end
