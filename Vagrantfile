Vagrant.configure("2") do |config|
  # (1..3).each do |i|
  #   config.vm.define "datanode#{i}" do |datanode|
  #     datanode.vm.box = "debian/bookworm64"
  #     datanode.vm.provider "virtualbox" do |vb|
  #         vb.memory = 2048
  #         vb.cpus = 2
  #     end
  #     datanode.vm.hostname = "datanode#{i}"
  #     datanode.vm.network "private_network", ip: "10.0.0.#{16+i}", netmask:"255.255.255.0"
  #     datanode.vm.provision "shell", path: "./debian11-setup.sh"
  #     datanode.vm.provision "shell", path: "./provision-datanode.sh"
  #   end
  #   config.vm.define "master" do |master|
  #     master.vm.box = "debian/bookworm64"
  #     master.vm.provider "virtualbox" do |vb|
  #         vb.memory = 2048
  #         vb.cpus = 2
  #     end
  #     master.vm.hostname = "master"
  #     master.vm.network "private_network", ip: "10.0.0.32", netmask:"255.255.255.0"
  #     master.vm.provision "shell", path: "./debian11-setup.sh"
  #     master.vm.provision "shell", path: "./provision-master.sh"
  #   end
  config.vm.define "client" do |client|
    client.vm.box = "debian/bookworm64"
    client.vm.provider "virtualbox" do |vb|
        vb.memory = 2048
        vb.cpus = 2
    end
    client.vm.hostname = "client"
    client.vm.network "private_network", ip: "10.0.0.33", netmask:"255.255.255.0"
    client.vm.provision "shell", path: "./debian11-setup.sh"
    client.vm.provision "shell", path: "./provision-client.sh"
  end
end
