Vagrant.configure(2) do |config|

  config.vm.define :observium do |v|
    v.vm.box = "geerlingguy/centos6"

    v.vm.network "private_network", type: "dhcp"
    v.vm.network "forwarded_port", guest: 80, host: 8080
    v.vm.network "forwarded_port", guest: 443, host: 8443

    v.vm.hostname = "observium.vagrant.com"

    v.vm.provider :virtualbox do |p|
      p.memory = 2048
      p.customize ["modifyvm", :id, "--paravirtprovider", "kvm"]
    end
  end

  config.vm.provision "ansible" do |a|
    a.playbook = "tests/vagrant.yml"
    # a.start_at_task = "Copy my.cnf"
    # a.verbose = 'vv'
    # a.skip_tags = [ "download", "packages" ]
    # a.tags = [ "debug", "install" , "download" ]
    # a.tags = "selinux"
  end

end
