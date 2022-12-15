# <img src="https://raw.githubusercontent.com/CraftLR/workshop-git/main/src/main/resources/assets/logo.png" alt="class logo" class="logo"/> 

## La Rochelle Software Craftsmenship

* **Auteurs:**

  * [Sébastien NEDJAR](mailto:sebastien.nedjar@univ-amu.fr)

* **Besoin d'aide ?**

  * Consulter et/ou créér des [issues](https://github.com/CraftLR/workshop-git/issues).
  * [Email](mailto:sebastien.nedjar@univ-amu.fr) pour toutes questions autres.

## Aperçu du tutoriel et objectifs d'apprentissage

Commencer à écrire du code demande souvent de disposer d'un environnement de développement particulier avec des contraintes bien spécifique concernant les logiciels disponibles ainsi que leurs versions. Développer avec un environement assez portable pour ne plus avoir à se préoccuper ni de la machine que l'on utilise ni de sa configuration permet de gagner un temps précieux et de se concentrer sur l'essentiel, c'est à dire produire le code qui répondra au mieux aux besoins de l'utilisateur. 

Avec la démocratisation des conteneurs et leur meilleure intégration dans les différents outils, il est maintenant possible de disposer de tels environements de développement assez facilement. L'objectif de ce tutoriel est de vous faire découvrir comment mettre en place ces conteneurs de développement et surtout comment les utiliser de manière quasi-transparente avec un IDE.

La technologie présentée est celle des [Dev Container](https://code.visualstudio.com/docs/devcontainers/containers) originellement dévéloppée pour [Visual Studio Code](https://code.visualstudio.com/docs/) mais qui est aujourd'hui disponible pour les IDE JetBrains à travers l'application [JetBrains Gateway](https://www.jetbrains.com/fr-fr/remote-development/gateway/).

Pour gagner encore plus en souplesse et en rapidité, il est possible de lancer le conteneur de développement sur une machine distante en utilisant des outils tels que [Github Codespaces](https://github.com/features/codespaces) ou [Gitpod](https://www.gitpod.io/).

Dans ce tutoriel, vous allez voir comment ces énvironements peuvent être mis en place et configuré directement dans le dépot git de votre projet. Ainsi, toute personne voulant contribuer à votre travail n'aura rien de plus à faire qu'à ouvrir l'IDE pour commencer à contribuer.

## Conteneur de développement

Un conteneur de développement permet d'abstraire les dépendances et les outils d'un projet via l'utilisation de [Docker](https://www.docker.com/). Le pack d'extension [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack) de VS Code permet à l'IDE d'interagir directement avec le conteneur. Cela réduit considérablement le temps de démarrage d'un nouveau développeur, tout en réduisant le risque d'installations incorrectes ou de blocage lors de l'installation.

Un conteneur de développement est défini par un fichier `devcontainer.json` qui doit se trouver dans le dossier `.devcontainer` à la racine du projet. Dans ce fichier, sont définis les services requis, ainsi que la configuration spécifique de l'application. Une fois le conteneur construit, VS Code peut travailler directement à l'intérieur du conteneur, comme si vous développiez localement. 

Il y a beaucoup à savoir sur les Dev Container, mais le moyen le plus simple de démarrer est de tester sur un projet déjà configuré.

La première chose à faire est de créer un fork de ce dépôt. Pour ce faire, rendez-vous sur le lien suivant :

<https://classroom.github.com/a/EXCRjwgv>

GitHub va vous créer un dépôt contenant un fork de ce dépôt. Vous apparaîtrez automatiquement comme contributeur de ce projet pour y pousser votre travail. Clonez localement votre fork et ouvrez le avec Visual Studio Code.

