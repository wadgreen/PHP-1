# Un Fromage
Vous avez fait un exercice avec des fromages, un fichier JSON chargé en Ajax pour lister des fromages sur une page HTML.  
A partir de cette base, opérez deux étapes supplémentaires :  
  
# 1 - Charger les données depuis le serveur local Apache (PHP)  
Récupérez le fichier JSON depuis le serveur local Apache (http://localhost/votredossier). Vous aurez à gérer vos entêtes dans la requête pour autoriser ce chargement et peut-être autoriser le CROSS-DOMAIN (...)  
(Sympa, je vous donne une piste [JSON+PHP](https://www.w3schools.com/js/js_json_php.asp) )  
S'il vous faut plus d'informations, jeter un oeil vers file_get_contents, ça pourrait être utile.  
  
# Ajoutez un fromage dans le JSON  
Créez une page de formulaire avec des champs permettant de créer un nouveau fromage (un par champ du JSON initial). Vous avez le choix de la technologie.  
Ce fichier doit permettre de réécrire le fichier JSON pour tenir compte de l'ajout du fromage.  
  
### Un peu d'aide ?  
PHP est bourré de possibilités mais vous aurez quelques paramètres en prendre en compte :  
- fopen, fwrite, fclose vous seront très utiles,  
- apache est une utilisateur de votre système comme un autre. Vous risquez d'avoir un problème à réécrire un fichier sans les droits. Jetez un oeil vers www-data pour plus d'infos.  
  
D'autres questions ? Nous ne sommes pas bien loin.