Vagrant.configure(2) do |config|

  config.vm.define :observium do |v|
    v.vm.box = "geerlingguy/centos6"
    v.vm.network "private_network", type: "dhcp"
    v.vm.provider :virtualbox do |p|
      p.memory = 2048
    end
  end

  config.vm.provision "ansible" do |a|
    a.playbook = "../../playbooks/observium.yml"
  end

end