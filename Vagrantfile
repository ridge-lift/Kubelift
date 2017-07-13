# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://atlas.hashicorp.com/search.
  # config.vm.box = "base"

  # Disable automatic box update checking. If you disable this, then
  # boxes will only be checked for updates when the user runs
  # `vagrant box outdated`. This is not recommended.
  # config.vm.box_check_update = false

  # Create a forwarded port mapping which allows access to a specific port
  # within the machine from a port on the host machine. In the example below,
  # accessing "localhost:8080" will access port 80 on the guest machine.
  # config.vm.network "forwarded_port", guest: 80, host: 8080

  # Create a private network, which allows host-only access to the machine
  # using a specific IP.
  # config.vm.network "public_network", ip: "192.168.0.10"

  # Create a public network, which generally matched to bridged network.
  # Bridged networks make the machine appear as another physical device on
  # your network.
  # config.vm.network "public_network"

  # Share an additional folder to the guest VM. The first argument is
  # the path on the host to the actual folder. The second argument is
  # the path on the guest to mount the folder. And the optional third
  # argument is a set of non-required options.
  # config.vm.synced_folder "../data", "/vagrant_data"

  # Provider-specific configuration so you can fine-tune various
  # backing providers for Vagrant. These expose provider-specific options.
  # Example for VirtualBox:
  #
  # config.vm.provider "virtualbox" do |vb|
  #   # Display the VirtualBox GUI when booting the machine
  #   vb.gui = true
  #
  #   # Customize the amount of memory on the VM:
  #   vb.memory = "1024"
  # end
  #
  # View the documentation for the provider you are using for more
  # information on available options.

  # Define a Vagrant Push strategy for pushing to Atlas. Other push strategies
  # such as FTP and Heroku are also available. See the documentation at
  # https://docs.vagrantup.com/v2/push/atlas.html for more information.
  # config.push.define "atlas" do |push|
  #   push.app = "YOUR_ATLAS_USERNAME/YOUR_APPLICATION_NAME"
  # end

  # Enable provisioning with a shell script. Additional provisioners such as
  # Puppet, Chef, Ansible, Salt, and Docker are also available. Please see the
  # documentation for more information about their specific syntax and use.
  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y apache2
  # SHELL

# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
#Vagrant.configure("2") do |config|

    config.vm.define "AnsibleCS" do |AnsibleCS|
        AnsibleCS.vm.box = "centos/7"
        AnsibleCS.vm.hostname = "AnsibleCS"
        AnsibleCS.vm.network "private_network", ip: "192.168.0.5"
        AnsibleCS.vm.network "forwarded_port", guest: 80, host: 8080
        config.ssh.insert_key = false
    end

    config.vm.define "k8sm1" do |k8sm1|
        k8sm1.vm.box = "centos/7"
        k8sm1.vm.hostname = "k8sm1"
        k8sm1.vm.network "public_network", ip: "192.168.0.10"
    end

    config.vm.define "k8sm2" do |k8sm2|
        k8sm2.vm.box = "centos/7"
        k8sm2.vm.hostname = "k8sm2"
        k8sm2.vm.network "public_network", ip: "192.168.0.11"
    end

    config.vm.define "k8sm3" do |k8sm3|
        k8sm3.vm.box = "centos/7"
        k8sm3.vm.hostname = "k8sm3"
        k8sm3.vm.network "public_network", ip: "192.168.0.12"
    end

    config.vm.define "k8sn1" do |k8sn1|
        k8sn1.vm.box = "centos/7"
        k8sn1.vm.hostname = "k8sn1"
        k8sn1.vm.network "public_network", ip: "192.168.0.50"
    end

    config.vm.define "k8sn2" do |k8sn2|
        k8sn2.vm.box = "centos/7"
        k8sn2.vm.hostname = "k8sn2"
        k8sn2.vm.network "public_network", ip: "192.168.0.51"
    end

    config.vm.define "k8sn3" do |k8sn3|
        k8sn3.vm.box = "centos/7"
        k8sn3.vm.hostname = "k8sn3"
        k8sn3.vm.network "public_network", ip: "192.168.0.52"
    end

    config.vm.define "k8sn4" do |k8sn4|
        k8sn4.vm.box = "centos/7"
        k8sn4.vm.hostname = "k8sn4"
        k8sn4.vm.network "public_network", ip: "192.168.0.53"
    end

    config.vm.define "k8sn5" do |k8sn5|
        k8sn5.vm.box = "centos/7"
        k8sn5.vm.hostname = "k8sn5"
        k8sn5.vm.network "public_network", ip: "192.168.0.54"
    end

    config.vm.define "k8sn6" do |k8sn6|
        k8sn6.vm.box = "centos/7"
        k8sn6.vm.hostname = "k8sn6"
        k8sn6.vm.network "public_network", ip: "192.168.0.55"
    end

end
