Vagrant.configure("2") do |config|
  config.vm.box = "ryanmaclean/openbsd-6.0"
  config.vm.box_version = "1.0.0"

  config.vm.provision "shell", path: "bootstrap.sh"
end
