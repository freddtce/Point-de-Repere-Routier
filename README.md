## Description du schéma
Ce schéma décrit le format d'échange des Points de Repère Routiers (PR) qui a été élaboré par La communauté des Conseils Départementaux d'Auvergne Rhône Alpes.
Le but de la communauté est de réfléchir à la création de différents formats afin de pouvoir facilement échanger/partager les données que chaque Conseil Départemental produit., de partager les expériences,d'échanger les pratiques...

Ce format permettra aux membres de la communauté (et à tous ceux qui voudrons utiliser ce format) d'intégrer facilement les PR des départements voisins, sans perdre un temps précieux à la découverte de la donnée.

L'idée est aussi de proposer le format d'échange régional comme une première pierre à la construction d'un standard national soit auprès du Conseil National de l'Information Géolocalisée - CNIG, soit auprès de la Délégation de la Sécurité Routière - DSR.

## Métadonnées du Format d'Echange
format : geopackage

encodage : utf8

type d'objet : ponctuel

date de mise à jour : AAAAMMJJ

## Précisions sur certains attributs

### identifiant
            il est fabriqué de la manière suivante : <dep>-<id_plo_usuel> 
            dep : 3 chiffres avec 0 en 1er chiffre pour les départements métropolitains
            id_plo_usuel : récupération des identifiants utilisés par chacun
            
### axe 
           Il renseigne le numéro de la route. Il est défini par délibération du conseil départemental mais ne requiert pas forcément un acte administratif (à minima un arrêté de mise en                                  service). 
            Dans le cas général, il est saisi sous la forme Dxxx où xxx est le numéro de la route en chiffres arabes et peut être suivi d’une lettre en majuscule ou minuscule et/ou de chiffres. 
            Certaines Métropoles utilisent la grammaire Mxxx
            
#### cas des giratoires : Dxxx_GIRyy  
            xxx est le numéro de la route en chiffres arabes et peut être suivi d’une lettre en majuscule ou minuscule
            yy le numéro du giratoire qui peut être un chiffre arabe, une lettre en majuscule ou une combinaison des 2
            Le séparateur est un underscore _  (tiret du 8)
            
#### cas des chaussées séparées : Dxxx_G 
            xxx est le numéro de la route en chiffres arabes et peut être suivi d’une lettre en majuscule ou minuscule
            Le séparateur est un underscore _  (tiret du 8)
            
#### cas des annexes ou indices : Dxxx-yy"
            xxx est le numéro de la route en chiffres arabes et peut être suivi d’une lettre en majuscule ou minuscule
            yy l’indice qui peut être un chiffre arabe, une lettre en majuscule ou minuscule, ou une combinaison des 2
            
#### le cas des bretelles n'est pas traité dans ce format PR

