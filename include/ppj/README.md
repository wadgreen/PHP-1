# PPJ aux taquets !!

!! Avant de faire cet exercice, vous devez avoir fait celui-ci : include/README.md !! 

## Encore des dossiers
Pierre, Paul et Jacquot vont avoir besoin d'un dossier intitulé "fonctions" situé à la racine du projet.<br>
Ils créeront la constante correspondante dans config/config.php.<br>
Ils s'aperçoivent qu'il en sera de même pour les classes...<br>

## Encore des include
Les compères remarquent également que leurs pages (accueil,produits,blog,contact,about) comportent du code en commun : les include de la balise head, nav, footer.<br>
Ils en concluent qu'ils pourraient très bien avoir des url de ce type : ppj/index.php?page=accueil. Il leur suffirait de récupérer le paramètre $_GET["page"] et inclure la page correspondante. Tout se ferait dans le fichier index.php !<br> Du coup, les pages pourraient être rangées dans un dossier template/pages, et les sous-parties (nav, footer...) dans un dossier templates/template-parts par exemple.<br>Il faudra penser à créer les constantes correspondantes !<br> De plus, avant d'inclure un fichier, il faudra vérifier que celui-ci existe...<br>
Si le fichier n'existe pas, on redirigera vers une page 404.<br>

## Chacun sa route
L'équipe ppj souhaite tenir à jour la liste des pages disponibles sur le site afin de mieux contrôler les valeurs du paramètre "page" de l'url ($_GET["page]).<br>
Le choix s'oriente vers un fichier routes.php contenant un tableau associatif (retourné par l'instruction return) avec pour clés les valeurs du paramètre "page" et pour valeur les noms des fichiers correspondants à inclure.<br> Par exemple, "accueil"=>"accueil.php". Cela permettra d'inclure un fichier dont le nom n'est pas forcément le même que le paramètre "page". On créera également une constante pour ce tableau.<br>On contrôlera l'existence de cette "route" dans routes.php avant d'inclure le fichier correspondant (en même temps que l'existence du fichier). Dans le cas contraire, on renverra une page 404.<br>