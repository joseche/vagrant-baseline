
Vagrant.configure(2) do |config|
  config.vm.box = "centos/7"
  # config.vm.network "private_network", ip: "10.1.1.20"
  # config.vm.hostname = "baselinehost"
  config.vm.provider "virtualbox" do |vb|
     vb.memory = "256"
  end
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "baseline.yml"
    ansible.sudo = true
  end
end
