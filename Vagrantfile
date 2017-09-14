# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

$UBUNTU_XENIAL_BOOTSTRAP_SCRIPT = <<SCRIPT
echo "Bootstrap Ubuntu 16.04 Machine"
apt install -y python aptitude
SCRIPT

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  # All setting on this level apply for all boxes.

  # Every Vagrant virtual environment requires a box to build upon.
  # A default setting is preferred
  config.vm.box = "ubuntu/xenial64"

  # Disable SharedFolder by default.
  config.vm.synced_folder ".", "/vagrant", disabled: true

  config.vm.define "ubuntu-12.04", primary: false, autostart: false do |node|
    node.vm.box = "ubuntu/precise64"
    node.vm.provider "virtualbox" do |vb|
      vb.name = "Ubuntu 12.04 LTS (Precise Pangolin)"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "ubuntu-14.04", primary: false, autostart: false do |node|
    node.vm.box = "ubuntu/trusty64"
    node.vm.provider "virtualbox" do |vb|
      vb.name = "Ubuntu 14.04 LTS (Trusty Tahr)"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "ubuntu-16.04", primary: false, autostart: false do |node|
    node.vm.box = "ubuntu/xenial64"
    node.vm.provider "virtualbox" do |vb|
      vb.name = "Ubuntu 16.04 LTS (Xenial Xerus)"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "debian-7", primary: false, autostart: false do |node|
    node.vm.box = "debian/wheezy64"
    node.vm.provider "virtualbox" do |vb|
      vb.name = "Debian 7 (Wheezy)"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "debian-8", primary: false, autostart: false do |node|
    node.vm.box = "debian/jessie64"
    node.vm.provider "virtualbox" do |vb|
      vb.name = "Debian 8 (Jessie)"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "debian-9", primary: false, autostart: false do |node|
    node.vm.box = "debian/stretch64"
    node.vm.provider "virtualbox" do |vb|
      vb.name = "Debian 9 (Stretch)"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "centos-6", primary: false, autostart: false do |node|
    node.vm.box = "centos/6"

    node.vm.provider "virtualbox" do |vb|
      vb.name = "CentOS/6"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "centos-7", primary: false, autostart: false do |node|
    node.vm.box = "centos/7"

    node.vm.provider "virtualbox" do |vb|
      vb.name = "CentOS/7"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "fedora-7", primary: false, autostart: false do |node|
    node.vm.box = "fedora/23-atomic-host"

    node.vm.provider "virtualbox" do |vb|
      vb.name = "Fedora 23"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "fedora-7", primary: false, autostart: false do |node|
    node.vm.box = "fedora/24-atomic-host"

    node.vm.provider "virtualbox" do |vb|
      vb.name = "Fedora 24"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "fedora-7", primary: false, autostart: false do |node|
    node.vm.box = "fedora/25-atomic-host"

    node.vm.provider "virtualbox" do |vb|
      vb.name = "Fedora 25"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "fedora-7", primary: false, autostart: false do |node|
    node.vm.box = "fedora/26-atomic-host"

    node.vm.provider "virtualbox" do |vb|
      vb.name = "Fedora 26"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "suse-11", primary: false, autostart: false do |node|
    node.vm.box = "suse/sles11sp3"

    node.vm.provider "virtualbox" do |vb|
      vb.name = "SLES 11"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "suse-12", primary: false, autostart: false do |node|
    node.vm.box = "suse/sles12sp2"

    node.vm.provider "virtualbox" do |vb|
      vb.name = "SLES 12"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "freebsd-10", primary: false, autostart: false do |node|
    node.vm.box = "freebsd/FreeBSD-10.3-stable"
    node.vm.provider "virtualbox" do |vb|
      vb.name = "FreeBSD 10"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

  config.vm.define "freebsd-11", primary: false, autostart: false do |node|
    node.vm.box = "freebsd/FreeBSD-11.1-stable"
    node.vm.provider "virtualbox" do |vb|
      vb.name = "FreeBSD 11"
      vb.memory = 1024
      vb.cpus = 1
      vb.customize ["modifyvm", :id,
                    "--cpuexecutioncap", "50",
                    "--groups", "/Vagrant/Base"
                   ]
    end
  end

end
