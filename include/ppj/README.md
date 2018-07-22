# PPJ aux taquets !!

!! Avant de faire cet exercice, vous devez avoir fait celui-ci : include/README.md !! 

## Encore des dossiers
Pierre, Paul et Jacquot vont avoir besoin d'un dossier intitulé "fonctions" situé à la racine du projet.<br>
Ils créeront la constante correspondante dans config/config.php.<br>
Ils s'aperçoivent qu'il en sera de même pour les classes...<br>

## Encore des include
Les compères remarquent également que leurs pages (accueil,produits,blog,contact,about) comportent du code en commun : les include de la balise head, nav, footer.<br>
Ils en concluent qu'ils pourraient très bien avoir des url de ce type : ppj/index.php?page=accueil. Il leur suffirait de récupérer le paramètre $_GET["page"] et inclure la page correspondante. Tout se ferait dans le fichier index.php !<br> Du coup, les pages pourraient être rangées dans un dossier template/pages, et les sous-parties (nav, footer...) dans un dossier templates/template-parts par exemple.<br>Il faudra penser à créer les constantes correspondantes !<br> De plus, avant d'inclure un fichier, il faudra vérifier que celui-ci existe...<br>
A suivre...