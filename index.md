---
title       : Introduction à la Data Science
subtitle    : Année scolaire 2014-2015
author      : Matthias Oehler
job         : Vice Président Data @Makazi
github      : {user: oehlr, repo: slide-introdatascience-session1}
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
logo        : logods.png
biglogo     : logo_polytech.jpg
--- { tpl: mkz-cols-thumbs, 
      description: ""}



## Sommaire - Session #1

*** { span: span3, img: nuclearidea.png}

### REVOLUTION

La Data science, c'est quoi exactement et quelles sont les diciplines auquelles cela fait référence ?

*** { span: span3, img: script.png}

### FONDAMENTAUX

Quels sont les grands principes de la Data science ?

*** { span: span3, img: cycle.png}

### PROCESSUS

Comment bien apréhender un sujet Data science et quels processus suivre afin d'en tirer profit ?

*** { span: span3, img: chart.png}

### PRODUIT

Vers une notion de Data produits. Quelques exemples ?








--- &mkz-section2 bg:#00B7BE img:white_nuclearidea.png

# <span style="font-weight:100">DATA</span> REVOLUTION







---  { tpl: slide,
       description: "Ces dernieres années, <b>Big Data</b> et <b>Data science</b> sont devenus la solution à tous les problèmes."}

## Qui a besoin de Data Science ?

<center>
<img width="70%" alt="DataScienceDisciplines" src="assets/img/bor55.png" />
</center>





---  { tpl: slide,
       description: "La Data science est composée de plusieurs expertises."}

## Data Science : qu'est ce que c'est exactement ?

<center>
  <a title="By Calvin.Andrus (Own work) [CC-BY-SA-3.0 (http://creativecommons.org/licenses/by-sa/3.0)], via Wikimedia Commons" href="http://commons.wikimedia.org/wiki/File%3ADataScienceDisciplines.png">
    <img width="65%" alt="DataScienceDisciplines" src="http://upload.wikimedia.org/wikipedia/commons/4/44/DataScienceDisciplines.png"/>
  </a>
</center>





---  { tpl: slide,
       description: "Le data scientist est la personne capable d'identifier/solutionner les problèmes pouvant étre résolus par les données."}

## Les data scientists

### Le data scientist :

- est un magicien

<br />
- est souvent au coeur d'une équipe multi-diciplinaire

<br />
- doit comprendre les contraintes de tous et s'adapter

<br />
- ~~sait~~ doit expliquer son métier

<br />
- à le metier le plus sexy du siecle (Harvard Business Review) 



--- { tpl: slide, 
      description: "<p>Le CRM et le Marketing sont les domaines d'expertises les plus courants.</p>"}

## Domaines d'applications

<img src="assets/fig/domainplot.png" title="plot of chunk domainplot" alt="plot of chunk domainplot" style="display: block; margin: auto;" />







--- { tpl: slide, 
      description: "<p>R et Python sont les langages de programmation préférés des Data scientists.</p>"}

## Langages de programmation utilisés

<img src="assets/fig/languageplot.png" title="plot of chunk languageplot" alt="plot of chunk languageplot" style="display: block; margin: auto;" />





--- { tpl: mkz-cols-panels, 
      description: "<p>Répartition des algorithmes mathématiques en grandes familles</p>"}

## Les grandes familles d'algorithmes

*** {class: span4}

### Supervisés

> - Regression
> - Decision Trees
> - Neural Nets
> - SVM
> - Bayesian Nets
> - Genetic Algorithms
> - Rules induction
> - Autres ...

*** {class: span4}

### Non Supervisés

> - ACP
> - ACM
> - Kohonen
> - Text mining
> - Bayesian Nets
> - Social Network
> - Autres ...


*** {class: span4}

### Associations

> - Association rules
> - Social Networks
> - Link Analysis
> - Collaborative filtering
> - Look alike
> - Autres ...




--- { tpl: slide, 
      description: "<p>Les algorithmes les plus utilisés par les Data Scientist sont les Regressions, les arbres de décisions et le clustering.</p>"}

## Utilisation des algorithmes

<img src="assets/fig/methodeplot.png" title="plot of chunk methodeplot" alt="plot of chunk methodeplot" style="display: block; margin: auto;" />







--- &mkz-section2 bg:#FE5745 img:book_white.png

# <span style="font-weight:100">DATA</span> FONDAMENTAUX








--- { tpl: mkz-rows-thumbs, 
      description: "<p>Ce qu'il faut connaitre</p>"}

## Environnements techniques

*** {height: "30%", img: cloud.png}

### Cloud computing

IaaS, PaaS, SaaS, DaaS : comment tout est devenu un "Service" stocké dans les nuages.

*** {height: "30%", img: node.png}

### Systemes distribués & Map reduce

Hadoop, HDFS, Hive, MapR : comment faire basculer les traitements analytics sur une architecture scalable.

*** {height: "30%", img: db.png}

### NoSQL

Big Table, MongoDB, Hbase, CouchDB : comment les sytemes de gestion de base de données ont ils évolués.






--- { tpl: mkz-cols, 
      description: "<p></p>"}

## Le Cloud Computing

*** {class: span8}

<center>
<img width="75%" alt="cloud" src="assets/img/cloud.jpg" />
</center>

*** {class: span4}

<h4 class="content-title">Grand public :</h4>

- Gmail
- Dropbox
- iCloud
- Flickr
- et des centaines...

<h4 class="content-title">Data sciences :</h4>

- <a href="https://rstudio-dev.rm-rf.io:1480/">RStudio</a>
- yhat
- Dataiku
- autre ?






--- { tpl: mkz-rows-callout, 
      description: "<p>Avantages et inconvenients du cloud computing pour la Data science</p>"}

## Le Cloud Computing et la Data science

*** {height: "45%", type: success}

### Avantages

- Simplicité de mise en place ne necessitant qu'une très faible intervention des services technique 
- Bénéficier d'une puissance de calcul elastique grâce à la virtualisation
- Maitrise des couts grâce au "Pay per use"
- Pouvoir accéder à ses algorithmes où que l'on soit

*** {height: "45%", type: danger}

### Inconvénients

- Couteux sur le long terme (abonnement), même si la logique de calcul est assez complexe (electricité, maintenance, renouvellement de park, ...)
- Dépendance forte à un tiers
- Pour des questions juridiques, l'utilisation du cloud computing peut être tout simplement impossible





--- { tpl: slide, 
      description: "<p>Vue conceptuelle</p>"}

## Systemes distribués & Map Reduce

<center>
<img width="70%" alt="DataScienceDisciplines" src="http://www.glennklockwood.com/di/mapreduce-workflow.png" />
</center>






--- { tpl: mkz-rows-callout, 
      description: "<p>Avantages et inconvenients du distribué pour la Data science</p>"}

## Les environnements distribués et la Data science

*** {height: "45%", type: success}

### Avantages

- Possibilité de stoquer et exploiter une volumétrie de donnée gigantesque () autant de descripteur pouvant service à un modèle prédictif)
- La volumétrie des données n'est plus réellement un problème. Les algorithmes fonctionnant sur 1 000 lignes fonctionneront sur 10^9 lignes
- Emergence de nouvelles approches méthodologiques et de nouveaux algorithmes

*** {height: "45%", type: danger}

### Inconvénients

- Le stockage de la données a repris l'avantage sur l'analyse des données. Une données bien souvent inexploitable en l'état et bien trop mal struturée.
- Quid de la pertinence d'utiliser un si gros volume de données vs. des échantillonages
- Demande bien souvent une refonte complète des algorithmes traditionnels pour fonctionner en distribué






--- { tpl: mkz-cols, 
      description: "<p>Les base de données NoSQL ont été spécialement conçu pour fournir des solutions de stockage de données de hautes performances et évolutives</p>"}

## Les bases de données NoSQL

*** {class: "span5"}

### Pourquoi le NoSQL ?

- Une solution "simple" pour répondre aux problématiques de volumétrie et de non structuration de la donnée.

<br />
- Moyennant certains compromis sur les fondements mêmes des SGBD :
  -  Atomicité
  -  Consistence
  -  Durabilité

<br />
- <b>Objectifs</b> : Scalabilité et haute disponibilité

*** {class: "span1"}


*** {class: "span5"}

### Grandes familles des BDD NoSQL :

- <b>Clé / valeur</b> : Ex. <a href="http://try.redis.io/">Redis</a>

- <b>Orientées documents</b> : Ex. <a href="http://www.mongodb.org/">MongoDB</a>

- <b>Orientées graphes</b> : Ex. <a href="http://neo4j.com/">Neo4J</a>

- <b>Orientées colonnes</b> : Ex. <a href="http://cassandra.apache.org/">Cassandra</a> 

La grande majorité de ces projets sont en Open Source, voir gratuit. Profitez en !

*** {class: "span1"}








--- { tpl: mkz-rows-callout, 
      description: "<p>Avantages et inconvenients des base NoSQL pour la Data science</p>"}

## Les BDD NoSQL et la Data science

*** {height: "45%", type: success}

### Avantages

- Scalabilité
- Données non structurée
- Données naturellemnt connecté (réseaux sociaux)

*** {height: "45%", type: danger}

### Inconvénients

- Gère mal les relations
- Structuration de la donnée dépendant de l'utilisation qui en est faite
- Non adapté en cas de besoin de requétage fort (schemaless) ou complexe




--- .segue .quote .dark

<q>Un data scientist est meilleur en statistique que n'importe quel développeur et meilleur en développement que n'importe quel statisticien</q>

<style>
.dark q {
  color: white;
}
</style>










--- &mkz-section2 bg:#FBCEB6  img:cycle_white.png

# <span style="font-weight:100">DATA</span> PROCESS






--- { tpl: slide,
      description: "<p>Les projets Data Science étant souvent très chronophages, il est important de structurer son travail.</p>"
    }

## Des processus : Pourquoi ?

- "Comment pourrais-je atteindre mon objectif ? En combien de temps ? Combien cela me coutera ?"

<br />
- "Mes données ? Je ne sais pas je vais voir avec mon DSI." 

<br />
- "Comment ca je ne peux pas l'àge et la civilité mes meilleurs clients ? Il fallait collecter l'information ?"

<br />
- "Quelles sont les règles qui permettent de prédire cela ? Non non, je ne veux pas que l'on utilise cette donnée."

<br />
- "Combien cela me rapportera ?"

<br />

<div class="alert alert-info" role="alert"><b>Conseil :</b> Procéder étape par étape</div>







---

## Le processus CRISP-DM

<center>
<img width="55%" alt="DataScienceDisciplines" src="assets/img/crispdm.png" />
</center>




---

## Processus émergent

<center>
<img width="70%" alt="DataScienceDisciplines" src="assets/img/Data_visualization_process_v1.png" />
</center>


--- .segue .quote .white

<q>Data Product : la fin des analyses statistiques<br /></q>

<style>
.dark q {
  color: white;
}
</style>







--- &mkz-section2 bg:#7F7FCF   img:chart_white.png

# <span style="font-weight:100">DATA</span> PRODUCT







--- { tpl: slide, 
      description: "Moteur de recommandation sur site" }

## Quelques exemples de Data Product

<center>
    <img width="50%" alt="fitbit" src="assets/img/macys-retargeting.png"/>
</center>




--- { tpl: slide, 
      description: "Moteur de suggestion" }

## Quelques exemples de Data Product

<center>
    <img width="50%" alt="fitbit" src="assets/img/linkedin.jpg"/>
</center>






--- { tpl: slide, 
      description: "Recherche d'image similaire" }

## Quelques exemples de Data Product

<center>
    <img width="50%" alt="fitbit" src="assets/img/similar.jpg"/>
</center>




--- { tpl: slide, 
      description: "Recherche de musique" }

## Quelques exemples de Data Product

<center>
    <img width="50%" alt="fitbit" src="assets/img/shazam.jpg"/>
</center>



--- { tpl: slide, 
      description: "Recommandation de style vestimentaire" }

## Quelques exemples de Data Product

<center>
    <img width="50%" alt="fitbit" src="assets/img/chic-type.jpg"/>
</center>




--- { tpl: slide, 
      description: "Recommandation de film" }

## Quelques exemples de Data Product

<center>
    <img width="50%" alt="fitbit" src="assets/img/netflix.jpg"/>
</center>




--- { tpl: slide, 
      description: "Prediction de la prochaine action importante" }

## Quelques exemples de Data Product

<center>
    <img width="50%" alt="fitbit" src="assets/img/google-now-cards.jpg"/>
</center>




--- { tpl: slide, 
      description: "Suivi des performances personnelles" }

## Quelques exemples de Data Product

<center>
    <img width="70%" alt="fitbit" src="assets/img/fitbit.jpg"/>
</center>








--- .segue .quote .white

<q>Par où commencer ?</q>

<style>
.dark q {
  color: white;
}
</style>


--- { tpl: slide, 
      description: "<p>Dans un contexte où les algorithmes sont de plus en plus utilisés au quotidien il devient indispensable de suivre une logique 'produit'</p>" }

## Les 3P

- Au dela d'une simple analyse statistique, le Data Product a pour vocation d'ètre <b>réutilisé, partagé, mesuré, amélioré</b><br /><br />

- Le Data scientist a (aussi) un casquette de développeur. Ainsi il doit savoir :
  - <b>Packager</b> : Capitaliser sur un travail déjà effectué, rentabiliser le temps passé (R&D) <br /><br />
  - <b>Partager</b> : Le travail collaboratif <br /><br />
  - <b>Publier</b> : Mettre en production son code <br /><br />

- Créer son propre Package, le partager sur Github et le faire tester


--- { tpl: slide, 
      description: "<p></p>" }

## Proposition pour le TP

- Création d'un package

<br />
- Récupération de données via Webservice

<br />
- Analyse de données de type "Document" (twitter)

<br />
- Publication













--- {
 tpl: thankyou,
 social: [{title: email, href: "moehler@makazi.com"}, {title: github, href: "https://github.com/OehlR"}]
}

## Merci

<div stype="color:#FFFFFF">Pour plus d'information, contactez moi !</div>



---

