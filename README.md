# terraform_vagrant sur windows ou Linux
# Dans ce projet j'ai deux VM créer avec l'outil VAGRANT
# Decompresser les deux fichiers vous trouverez deux dossiers
# chacun ayant un fichier VAGRANFILE, l'une étant VM source et
# l'autre VM target (destination).
# Pour les lancer faut aller dans chacun des dossiers et lancer
# la commande vagrant up (faut lancer les deux vm dans deux terminaux distincts) 
# pour accèder aux vm faites : vagrant ssh 
# Sur la machine source vous allez trouvez un fichier dans projetTerraform/main.tf
# ( terraform est déja installé sur la vm source)
# le main.tf à pour role d'installer le package nginx sur la vm target, pour ce faire  
# faut lancer : terraform init puis terraform apply --auto-approve 
# enfin aller sur la vm target et taper systemctl ngnix status ou bien
# curl http://192.168.33.11 pour voir si tout va bien.
# pour sortir des vm sudo init 0 ou bien exit puis vagrant halt 



