# Scrum chez Kisio Digital


##Pourquoi ce livret ?
Agile, oui, mais made in Kisio Digital.
L’agilité est un mot en vogue ces derniers temps et il est possible que vous en ayez déjà fait. Ce livret permettra aux plus agiles comme aux débutants de s’y retrouver dans notre implémentation.
Bonne lecture.

##Comment travaille-t-on chez KD ?
###Pourquoi l’Agile ?
L'Agilité est une approche pragmatique, adaptative et  itérative pour l'accompagnement du développement de projets/produits. Ainsi par des pratiques (Scrum, Kanban, Lean Start-Up …) permettant une augmentation de la satisfaction et de la qualité, elles entraînent une amélioration du Time-To-Market et de la collaboration avec les clients.
L’Agilité est un état d’esprit permettant à une entreprise de faire les premiers pas vers l’entreprise libérée mettant ainsi le bonheur des collaborateurs au centre de la création de valeur.

##Historique
```
En février 2001, aux États-Unis, dix-sept spécialistes du développement logiciel se sont réunis pour débattre du thème unificateur de leurs approches respectives, dites "agiles". 
```
Les plus connus d'entre eux étaient :

- Ward Cunningham, inventeur du Wiki via WikiWikiWeb,
- Kent Beck, père de l'eXtreme Programming et cofondateur de JUnit, 
- Ken Schwaber et Jeff Sutherland, fondateurs de Scrum, 
- Jim Highsmith, prônant l'Adaptive Software Development, 
- Alistair Cockburn pour la méthode Crystal Clear, 
- Martin Fowler, Dave Thomas et Arie van Bennekum pour DSDM (Dynamic System Development Method) la version anglaise du RAD (développement rapide d'applications)

Ces 17 experts venant tous d'horizons différents réussirent à extraire de leurs concepts respectifs des critères pour définir une nouvelle façon de développer des logiciels.

De cette réunion devait émerger le Manifeste agile, considéré comme la définition canonique du développement agile et de ses principes sous-jacents.

L'origine des approches agiles est liée à l'instabilité de l'environnement technologique et au fait que le client est souvent dans l'incapacité de définir ses besoins de manière exhaustive dès le début du projet. Le terme « agile » fait ainsi référence à la capacité d'adaptation aux changements de contexte et aux modifications de spécifications intervenant pendant le processus de développement.


#Le manifeste
##Les valeurs
Nous découvrons comment mieux développer des logiciels par la pratique et en aidant les autres à le faire. Ces expériences nous ont amenés à valoriser :

- Les individus et leurs interactions plus que les processus et les outils
- Des logiciels opérationnels plus qu’une documentation exhaustive
- La collaboration avec les clients plus que la négociation contractuelle
- L’adaptation au changement plus que le suivi d’un plan

Nous reconnaissons la valeur des seconds éléments, mais privilégions les premiers.

##Les principes

1.	Notre plus haute priorité est de satisfaire le client en livrant rapidement et régulièrement des fonctionnalités à grande valeur ajoutée.

2.	Accueillez positivement les changements de besoins, même tard dans le projet. Les processus agiles exploitent le changement pour donner un avantage compétitif au client.

3.	Livrez fréquemment un logiciel opérationnel avec des cycles de quelques semaines à quelques mois et une préférence pour les plus courts.

4.	Les utilisateurs ou leurs représentants et les développeurs doivent travailler ensemble quotidiennement tout au long du projet.

5.	Réalisez les projets avec des personnes motivées. Fournissez-leur l’environnement et le soutien dont elles ont besoin et faites-leur confiance pour atteindre les objectifs fixés.

6.	La méthode la plus simple et la plus efficace pour transmettre de l’information à l'équipe de développement et à l’intérieur de celle-ci est le dialogue en face à face.

7.	Un logiciel opérationnel est la principale mesure d’avancement.

8.	Les processus agiles encouragent un rythme de développement soutenable. Ensemble, les commanditaires, les développeurs et les utilisateurs devraient être capables de maintenir indéfiniment un rythme constant.

9.	Une attention continue conduit à l'excellence technique et à une bonne conception renforce l’agilité.

10.	La simplicité – c’est-à-dire l’art de minimiser la quantité de travail inutile – est essentielle.

11.	Les meilleures architectures, spécifications et conceptions émergent d'équipes auto-organisées.

12.	À intervalles réguliers, l'équipe réfléchit aux moyens de devenir plus efficace, puis règle et modifie son comportement en conséquence.


##Les outils pour l'Agilité
###Planning poker

Une pratique ludique d'estimation utilisée par les équipes Scrum.

Autour de la table, chacun dispose d'un jeu de cartes représentant des valeurs typiques pour l'estimation en points d'une user story. Le Product Owner présente rapidement l'objectif d'une story. Chacun choisit ensuite une estimation, en silence, et prépare la carte correspondante face cachée. Lorsque tout le monde est prêt, on retourne les cartes simultanément et on donne lecture des estimations. 

S'il y a concensus sur l’estimation exemple (3, 3, 3, 5), on garde le score partagé (3). Par contre s’il existe un delta entre les scores (1,1,2,5) ou encore (3,5,5,13), les membres de l'équipe ayant donné l’estimation la plus basse et la plus haute sont invités à expliquer leur raisonnement; après une brève discussion, on cherche à émettre une estimation faisant consensus, éventuellement en répétant le jeu.

L’objectif de cette pratique est de provoquer la discution entre les membres de l’équipe de réalisation. Il n’y a pas de note juste et la simultanéité de la découverte des cartes est essentielle pour que les plus juniors ne soient pas influencés par les seniors. Elle permet également de voir si une story est complètement incomprise (?), ou insignifiante (0) ou inestimable en l’état (40,100) pas assez affinée.

Ce qu’on recherche c’est un <b>consensus</b> car c’est l’équipe et non pas un individu qui s’engage sur cette estimation.

<img src="https://github.com/lesagilitateurs/Scrum/blob/master/planning-poker-deck.jpg" height="200">


### TDD (Test-driven developpement)
Le terme TDD ou (développement piloté par les tests) désigne une technique de développement qui entremêle l'écriture de tests unitaires, la programmation et l'activité de remaniement. 
Elle propose les règles suivantes: 
- créer un seul test unitaire décrivant un aspect du programme 
- s'assurer, en l'exécutant, que ce test échoue pour les bonnes raisons 
- écrire juste assez de code, le plus simple possible, pour que ce test passe 
- remanier le code autant que nécessaire pour se conformer aux critères de simplicité 
- recommencer, en accumulant les tests au fur et à mesure 

La pratique est indissociable de la famille d'outils de tests xUnit, à qui elle doit son vocabulaire: 
- "barre verte" signifie que l'ensemble des tests unitaires accumulés passent avec succès.
- "barre rouge" signifie qu'au moins un test est en échec. (L'échec d'un unique test suffit à déclencher l'affichage rouge, avec sa connotation d'alerte: cette tolérance zéro reflète la philosophie de l'outil et de la pratique.) 

L'expression "dérouler les tests" désigne le fait de lancer ou d'exécuter tous les tests accumulés ("suite" ou "batterie" de tests). 

Les tests contribuent à garantir la <b>qualité</b> du code produit.

<img src="https://github.com/lesagilitateurs/Scrum/blob/master/tdd.png" height="200">


### Code review (revue de code)
Pour fournir un logiciel de qualité, il est nécessaire de produire un code source de qualité. La revue de code permet d’identifier des bugs avant de les rencontrer au moyen d’une relecture du code source par un développeur expérimenté.
La mise en place d’une revue de code systématique pendant la phase de développement et de correction, les développeurs se responsabilisent encore plus, car ils savent que leur travail sera automatiquement évalué. Ce système permet d’améliorer la qualité du code source écrit. De plus, le relecteur pourra identifier des bugs ou des axes d’amélioration.

Il existe Trois processus de revue de code:
- Revue de code bloquante : tout développement doit être relu avant d’être commité dans le référentiel du code source. Ce mode est un frein au développement car certains développement peuvent se retrouver en attente d’une relecture de développement dont ils dépendent.
- Revue de code non-bloquante : tout code source commité dans le référentiel du source source doit être relu. Cette méthode permet au développeur de continuer son travail sans attendre la relecture. De même, le relecteur n’est pas obligé de se précipiter pour relire le code.
- Revue de code avec le développement par binôme : c’est une conséquence de l’eXtreme Programming. Cependant le travail en binôme influence le jugement du relecteur direct.


### Pair programming (Programmation en binôme ou binômage)

Deux programmeurs partagent un seul poste de travail (écran, clavier, souris), se répartissant les rôles entre un "conducteur" (aux commandes) et un "copilote" (surveillant l'écran et intervenant en cas de besoin), intervertissant les rôles fréquemment. 

L'un des principaux écueils à la pratique du binômage est la passivité. Lorsqu'on l'utilise conjointement avec le développement par les tests, une variante appelée "ping pong programming" favorise l'échange de rôles: l'un des deux programmeurs écrit un test unitaire qui échoue, puis passe le clavier à son collègue qui cherche alors à faire passer ce test, et peut alors à son tour écrire un test. Cette variante peut être utilisée soit pour des raisons pédagogiques, soit dans un esprit plus ludique par des programmeurs déjà confirmés.

Les bénéfices attendus sont les suivants:
- Une plus grande qualité des développements; "programmer à haute voix" conduit à mieux appréhender les complexités et les détails pernicieux, limitant ainsi le risque d'erreurs ou de se fourvoyer.
- Une meilleure diffusion des connaissances dans l'équipe, notamment lorsqu'un développeur peu familier d'un module travaille avec un autre qui le connaît mieux. 
- Une amélioration plus rapide des compétences des développeurs juniors, au contact des seniors.
- Une meilleure lisibilité du code.
- Une réduction de l'effort de coordination, puisqu'au lieu de N développeurs on est amené à coordonner N/2 binômes 
- Une meilleure capacité à rester concentrer et résister aux interruptions: lorsqu'un des deux membres du binôme doit s'interrompre, l'autre peut rester focalisé sur la tâche et aider son collègue à se reconcentrer ensuite.
- Implique une revue de code directe et limite donc les risques de bug

<img src="https://github.com/lesagilitateurs/Scrum/blob/master/pair-programming.jpg" height="200">


