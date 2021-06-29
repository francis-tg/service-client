# Système de service client
## Les procédés

# Methode 1

### Démarrer le serveur local PHP par le fichier -> server

````cmd
-> php server
````
### Ou créer un server localhost qui prend à la racine -> **/**
## Exemple:
````cmd
http://fancis.tg
http://fancis.tg/
````
## Démarrer avec le server local #PHP

````cmd
-> php server
````

## Le dossier de traitement est #public

### NB: Pour cette methode il vous faut quelques driver...

# Methode 2

<h5> visiter le fichier xampp/apache/conf/extra/httpd-vhosts.conf et ajouter</h5>

````ini
<VirtualHost *:80>
    DocumentRoot "C:/xampp2/htdocs"
    ServerName localhost
    ##ErrorLog "logs/dummy-host2.example.com-error.log"
    ##CustomLog "logs/dummy-host2.example.com-access.log" common
</VirtualHost>

<VirtualHost *:80>
	ServerName client.service.com
	DocumentRoot "C:/xampp2/htdocs/wait/public/"
</VirtualHost>

````
<h5> Visitez C:\Windows\System32\drivers\etc ajouter <h5>

````ini
127.0.0.8   client.service.com
::1         client.service.com
````
"# service-client" 
