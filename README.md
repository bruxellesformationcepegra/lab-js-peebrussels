# Où faire pipi à Bruxelles ? 

## Pitch

Le but est de créer une page qui affiche une carte de Bruxelles avec l'indication des toilettes et urinoirs publics. Demo sur http://peebrussels.azurewebsites.net (si ça ne marche pas, dites-le moi, c'est que le site est arrêté)

## Tâches

- Créez une page HTML et affichez une carte Google Maps centrée sur Bruxelles-Centre grâce au plugin Gmaps.js (http://hpneo.github.io/gmaps/examples/markers.html)
- L'Open Data de la ville de Bruxelles offre 2 services pour vous aider: [les urinoirs publics](http://opendata.bruxelles.be/explore/dataset/bruxelles_urinoirs_publics/) et les [toilettes publiques](http://opendata.bruxelles.be/explore/dataset/bruxelles_toilettes_publiques/)
- Faites un appel AJAX pour chacun de ses services; ils renvoient une liste de points avec pour chacun les coordonnées géographiques et une description. La structure des données renvoyées est consultable sur le site de l'Open Data, regardez: 

```javascript
"fields":{

    "geo_coordinates":[
        50.853945961372055,
        4.346762248410073
    ]
    ,
    "description":"Toilette Quai à la Houille"

}
```
- Créez des *marker* sur la carte pour chacun des points en mettant la description dans l'infoWindow

## Pour ceux qui veulent aller + loin

Faites du **geocoding** pour récupérer l'adresse exacte de l'urinoir/toilette quand vous le/la sélectionnez

**Happy pee**