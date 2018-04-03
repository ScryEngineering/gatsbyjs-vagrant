Vagrant.configure("2") do |config|
  config.vm.box = "alpine/alpine64"
  config.vm.network "forwarded_port", guest: 8000, host: 8000
  config.vm.provider "virtualbox" do |vb|
    # Display the VirtualBox GUI when booting the machine
    vb.gui = true

    # Customize the amount of memory on the VM:
    vb.memory = "1024"
  end
  config.vm.provision "shell", inline: <<-SHELL
    apk add nodejs
    apk add yarn
    yarn global add gatsby-cli
  SHELL
end
