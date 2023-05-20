---
title: PYM's life website README
author: Pierre-Yves Martin
---

[![Netlify Status](https://api.netlify.com/api/v1/badges/3c947407-d8d9-4840-b216-78a24967fcbc/deploy-status)](https://app.netlify.com/sites/a-pym-s-life/deploys)

Ce projet est mon site web personnel. Initialement, il s'appuyais sur [Jeckyl](https://jekyllrb.com) puis [Pelican](https://getpelican.com) et maintenant [quarto](https://www.quarto.org).

## La technique

- [quarto](https://www.quarto.org), un générateur de site statique extrèmement flexible
- [Pandoc](https://pandoc.org/MANUAL.html) comme moteur de rendu très avancé du markdown avec plein d'extensions utile pour moi : formule de math en LaTeX, support des gif, notes de bas de page, support des emoji…
- un thème basé sur celui de [html5up.net](html5up.net) mais tout réécrit par mes soins à la mai
- [Netlify](https://netlify.com) pour le déploiement et l'hébergement (gros merci au [tuto de Mkco's Blog](https://mcko.me/en/how-to-deploy-pelican-to-netlify.html) d'ailleurs)

## Le contenu

Sinon niveau contenu, il y aura pas mal d'aventure authentiquement improbables, de la science débilement complexe et de la capoeira.

## TODO

### Nouvelles fonctionnalité

- [ ] ajouter un "estimated reading time" aux articles

### Contenus à ajouter

- [ ] ajouter des pages d'auteurs
  - [ ] Héloïse/Bambi
  - [ ] Zélie
  - [ ] Laura/Raptor
  - [x] PYM/Pirata
  - [ ] MRO
- [x] ajouter des pages pour chaque catégorie

### Corrections

### Outils et workflow

- [x] ajouter une une list "à faire" au README
- [x] passer des css aux scss
- [ ] passer tout le repo a [git lfs](https://git-lfs.github.com) (même d'historique)
- [ ] générer des pdf pour les pages de chansons de capoeira
