---
title: PYM's life website README
author: Pierre-Yves Martin
---

[![Netlify Status](https://api.netlify.com/api/v1/badges/3c947407-d8d9-4840-b216-78a24967fcbc/deploy-status)](https://app.netlify.com/sites/a-pym-s-life/deploys)

Ce projet est mon site web personnel. Initialement, il s'appuyais sur [Jeckyl](https://jekyllrb.com) mais maintenant je suis passé à [Pelican](https://getpelican.com).

## La technique

- [Pelican](https://getpelican.com), un générateur de site statique en langage [Python](https://www.python.org) (un de mes langage favori) vraiment très flexible
- [Pandoc](https://pandoc.org/MANUAL.html) comme moteur de rendu très avancé du markdown avec plein d'extensions utile pour moi : formule de math en LaTeX, support des gif, notes de bas de page, support des emoji…
- un thème basé sur celui de [html5up.net](html5up.net) mais tout réécrit par mes soins à la mai
- [Netlify](https://netlify.com) pour le déploiement et l'hébergement (gros merci au [tuto de Mkco's Blog](https://mcko.me/en/how-to-deploy-pelican-to-netlify.html) d'ailleurs)

## Le contenu

Sinon niveau contenu, il y aura pas mal d'aventure authentiquement improbables, de la science débilement complexe et de la capoeira.

## TODO

### Nouvelles fonctionnalité

- [ ] séparer le site et son contenu dans deux repositories différents
- [ ] ajouter un système de commentaire via la metadata comments (par défaut True) voir [le tuto](https://snipcart.com/blog/pelican-blog-tutorial-search-comments)
- [ ] ajouter la possibilité d'avoir des pages privées avec le plugin [Encrypt Pelican Content](https://github.com/mindcruzer/pelican-encrypt-content)
- [ ] ajouter une sitemap avec le plugin [Sitemap](https://github.com/pelican-plugins/sitemap)
- [ ] ajouter une licence globale et des licences spécifique pour chaque post (par défaut la licence globale grâce au plugin [Global licence](https://github.com/getpelican/pelican-plugins/tree/master/global_license))
- [ ] utiliser le plugin [Image Process](https://github.com/pelican-plugins/image-process) pour générer les thumb et les des versions adaptée à la résolution d'affichage pour chaque image (à part les gifs)
- [ ] remplacer le menu tags par un nuage de tags avec le plugin [Tag Cloud](https://github.com/pelican-plugins/tag-cloud)
- [ ] utiliser le plugin [pelican-seo](https://github.com/MaevaBrunelles/pelican-seo) qui gère le `robot.txt` et des schema `JSON-LD` pour les moteurs de recherche
- [ ] ajouter les articles suivants/précédents grâce au plugin [Neighboor Articles](https://github.com/pelican-plugins/neighbors) ou [Multi Neighbors](https://github.com/davidlesieur/multi_neighbors)
- [ ] ajouter un "estimated reading time" aux article (homepage, categories et article) peut-être avec le plugin [pelican-ert](https://github.com/nogaems/pelican-ert) ou [pelican-readtime](https://github.com/getpelican/pelican-plugins/tree/master/readtime)
- [ ] ajouter la gestion des évènements avec le plugin [Events](https://github.com/getpelican/pelican-plugins/tree/master/events) (pour l'academia)

### Contenus à ajouter

- [ ] ajouter une Twitter/OpenGraph card pour la homepage, les pages auteur, les pages categories, le template par défaut
- [ ] ajouter une page "about" qui explique que c'est un site statique à l'ancienne c.f. le message de MRO
- [ ] ajouter des pages d'auteurs (voir le plugin [Auto Pages](https://github.com/getpelican/pelican-plugins/tree/master/autopages)) :
  - [ ] Héloïse/Bambi
  - [ ] Zélie
  - [ ] Laura/Raptor
  - [ ] PYM/Pirata
  - [ ] MRO
- [ ] ajouter des pages pour chaque catégorie (voir le plugin [Auto Pages](https://github.com/getpelican/pelican-plugins/tree/master/autopages))
- [ ] ajouter la catégorie des posts sur les pages d'article
- [ ] faire une page d'aide sur le markdown spécifique à ce site

### Corrections

- [ ] ajouter les tags sur la page d'accueil, les pages de catégorie et les pages d'article
- [ ] corriger les contact sur la page d'accueil
- [ ] ajouter une favicon

### Outils et workflow

- [x] ajouter une une list "à faire" au README
- [ ] améliorer la gestion du js/css grâce au plugin [Web Assets](https://github.com/pelican-plugins/webassets)
- [ ] ajouter un [justfile](https://github.com/casey/just)
  - [ ] pour ajouter un nouvel article (à partir d'un modèle)
  - [ ] pour passer un article de draft/published
  - [ ] pour lister tous les posts
- [ ] documenter correctement le `pelicanconf.py` (en particulier les variable que j'ai ajoutées et préciser que tout ce qui est en majuscule est ajouté au contexte)
- [ ] passer tout le repo a [git lfs](https://git-lfs.github.com) (même d'historique)
- [ ] générer des pdf pour les pages de chansons de capoeira
- [ ] passer des css aux scss (le plugin [Web Assets](https://github.com/pelican-plugins/webassets) est surement le meilleur moyen)
- [ ] mettre à jour la conf de [Pandoc](https://pandoc.org/MANUAL.html) avec toutes les extensions utilisées explicitement
- [ ] valider les page avec le plugin [w3c_validate](https://github.com/getpelican/pelican-plugins/tree/master/w3c_validate) et ajouter ça au [pre-commit](https://pre-commit.com)
- [ ] ajouter une étape de vérification pour s'assurer que les pages se génèrent bien au [pre-commit](https://pre-commit.com)
