# Accès aux schémas d'armoires électriques par code QR

Solution web simple permettant à un technicien de maintenance de scanner un code QR collé sur une armoire électrique pour consulter sa fiche technique et ses schémas unifilaires depuis un smartphone.

Projet réalisé lors d'un stage technicien en milieu industriel pharmaceutique (3 juin au 2 juillet 2026), 3e année Génie Électrique, ENSIT.

## Mon travail

Ce projet comprend trois réalisations personnelles :

1. **Relevé sur site** de 10 armoires électriques détaillées dans deux locaux techniques (6 dans le local R+2, 4 dans le local Carthago), en présence du personnel de maintenance, avec l'identification des protections, des variateurs et des récepteurs alimentés. Onze coffrets d'automates du local R+2 sont repérés mais restent à détailler.
2. **Dessin des schémas unifilaires sous AutoCAD**, réalisé par mes soins, avec des conventions homogènes pour toutes les armoires. Les schémas sont regroupés dans deux plans d'ensemble (R+2 et Carthago) exportés en PDF vectoriel.
3. **Conception de la page web et des codes QR** donnant accès à ces plans depuis l'armoire.

## Principe

Scan du code QR de l'armoire → ouverture de la page web → consultation de la fiche technique → ouverture du plan PDF du local → zoom sur l'armoire concernée.

## Fonctionnalités

- Indicateur d'état de l'armoire (« En Service »)
- Fiche technique : localisation, tension nominale, courant nominal, indices IP/IK, norme
- Accès aux plans schématiques au format PDF, par local
- Code QR pour chaque plan, pour transférer la consultation de l'ordinateur au téléphone
- Bouton de signalement d'anomalie
- Mise en page adaptée au téléphone et à l'ordinateur (responsive)

## Technologies

- HTML5, CSS3, JavaScript
- AutoCAD : schémas unifilaires dessinés par moi-même, puis exportés en PDF vectoriel
- Codes QR générés à partir de l'adresse de la page ou du plan
- Hébergement statique

## Contenu du dépôt

```
index.html    Page web « Armoire Électrique »
README.md     Ce fichier
```

## Données non incluses

Les plans électriques de l'usine ne sont pas publiés dans ce dépôt : ce sont des documents internes. La page est fournie comme modèle, et les liens vers les PDF sont à adapter.

## Pistes d'évolution

- Un code QR par armoire, avec une fiche technique personnalisée
- Accès restreint au réseau interne ou protégé par authentification
- Liaison du bouton de signalement à la GMAO
- Historique des interventions et des révisions de plan

## Auteur

Abidi Wiem
