Vagrant.configure(2) do |config|
  config.vm.box = "centos/7"
  config.vm.provider "virtualbox" do |vb|
    vb.gui = true
    vb.memory = "1024"
  
    vb.customize ["modifyvm", :id, "--clipboard",   "bidirectional"]
    vb.customize ["modifyvm", :id, "--draganddrop", "bidirectional"]

  end
  config.vm.provision "shell", path: "provision.sh"
end
