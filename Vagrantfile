Vagrant.configure("2") do |config|
  # Utiliser l'image de la box Ubuntu 22.04
  config.vm.box = "bento/ubuntu-22.04"

  # Configurer l'adresse IP de la machine virtuelle
  config.vm.network "private_network", ip: "192.168.13.6"

  # Configurer le port redirigé
  config.vm.network "forwarded_port", guest: 80, host: 80

  # Configurer le dossier synchronisé
  config.vm.synced_folder "./dossier_DevOps", "/home/vagrant/dossier_DevOps"

  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y apache2
  # SHELL
end
