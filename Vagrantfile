VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define "vagrant2" do |vagrant2|
    vagrant2.vm.box = "ubuntu/focal64"
    vagrant2.vm.network "forwarded_port", guest: 80, host: 8000
    vagrant2.vm.network "forwarded_port", guest: 443, host: 8443
    vagrant2.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end
end
