Questo playbook installa e configura Telegraf su Ubuntu o Debian via .deb file.

Per configurare lo script è necessario:
1) Popolare il file hosts.yaml con le macchine target differenziate per gruppi
2) Popolare il file vars.yaml come da commenti
3) Popolare la directory configuration-files, similmente a come fatto per il gruppo d'esempio. Ciascun gruppo deve avere la sua subdirectory così come dichiarata nelle variabili dedicate nel file hosts

Per lanciare lo script: 
ansible-playbook -i hosts.yaml site.yaml --key-file key.pem

Si noti che, da requisiti, a tutte le macchine si accede con la stessa ssh key.
