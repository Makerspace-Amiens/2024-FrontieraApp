---
layout: default
nav_order: 5
title: Conception et prototypage
---
| Index | Règles | Conception | Etudes | Mini-jeux | Objectifs |
| --------- | --------- | --------- | --------- | --------- | --------- |
| <details><summary></summary>[°](https://github.com/Makerspace-Amiens/2024-FrontieraApp/blob/main/docs/index.md)</details> | <details><summary></summary>[°](https://github.com/Makerspace-Amiens/2024-FrontieraApp/blob/main/docs/R%C3%A8gles.md)</details> | <details><summary></summary>[°](https://github.com/Makerspace-Amiens/2024-FrontieraApp/blob/main/docs/conception.md)</details> | <details><summary></summary>[°](https://github.com/Makerspace-Amiens/2024-FrontieraApp/blob/main/docs/etudes.md)</details> | <details><summary></summary>[°](https://github.com/Makerspace-Amiens/2024-FrontieraApp/blob/main/docs/mini-jeux.md)</details> | <details><summary></summary>[°](https://github.com/Makerspace-Amiens/2024-FrontieraApp/blob/main/docs/objectifs.md)</details> |

# Conception et prototypage
Frontiera est un jeu 2D disponible sur nagivateur, et réalisé sous le moteur de jeu Unity.

## Interface graphique
L'interface graphique de Frontiera est conçue à l'aide de sprites déssinées en pixelart.  
Le pixelart est une forme d'art numérique qui va nous permettre de créer une forme à partir de pixels. Afin de réaliser ces sprites il existe de nombreux logiciels.
* **Création des sprites**

  Pour la réalisation des différentes sprites de jeu, nous avons choisi Piskel qui est un logiciel de dessin gratuit et facile d'accès spécifique au pixelart. Les premières sprites de notre jeu sont celles du dé permettant de déterminer le nombre de cases de départ, et les différents états de cases du plateau possible.
  
  Une fois toutes ces sprites crées il faut réaliser ce qu'ont appelle une *spritesheet*. Il s'agit d'une "feuille" sur laquelle nous allons regrouper toutes nos différentes sprites afin d'en faire un seul et même fichier. Cela permet une importation et une gestion beaucoup plus simple.
  
  Exemple de sprite et de spritesheet ci-dessous :
  
   ![screen_dé](https://github.com/Makerspace-Amiens/2024-FrontieraApp/assets/158062961/d11bde4b-45fe-41c6-84dc-b878b79c3e3e)
  
   ![screen_spritesheet_dé](https://github.com/Makerspace-Amiens/2024-FrontieraApp/assets/158062961/70be1294-1a30-4364-ab11-7ddf08d37c63)

* **Importation sur Unity**
l'étape suivant la création des sprites est leur importation sur Unity. 
  
  
## Organisation de la programmation

Avant d'entamer la programmation de notre jeu, nous avons d'abord procéder à une phase de réflexion. Nous avons défini et créer différents organigrammes qui retrace le déroulement du jeu avec une partie complète.  


![Organigramme partie](https://github.com/Makerspace-Amiens/2024-FrontieraApp/assets/158062961/6672c83a-fbe2-4252-b250-8953576d86ba)  



* *Programmation du plateau* :

  Les premiers prototypes du plateau ont eté réalisés grâce au logiciel Processing. Il nous a permis d'avoir un premier aperçu de notre plateau avec les différentes cases. Grâce à ça, nous avons pû trouver la meilleure manière de gérer les coordonnées de nos différentes cases.  

  ![Prototype plateau couleur](https://github.com/Makerspace-Amiens/2024-FrontieraApp/assets/158062961/05750076-c588-41d7-b03f-be6aeb16d0fc)

  
* *Programmation du Menu Démarrer* :

  Le premier prototype du menu à également été réaliser sur Processing. Il reprend les éléments importants à savoir un bouton "Nouvelle partie", des options ainsi qu'un bouton quitter.
  
  
  ![Prototype menu](https://github.com/Makerspace-Amiens/2024-FrontieraApp/assets/158062961/a7b8a378-d617-4961-86e3-6cc99f58d3c4)


  
* *Programmation des éléments indépendants* :

  
* *Programmation des mini-jeux* :  
  Frontiera possède une variété de mini-jeux qui ont tous nécéssités une approche différente. 

## Tests 

* *Mini-jeu Questions - Réponses*  
  Le premier prototype de ce mini-jeu ce présente comme ceci:  

![image](https://github.com/Makerspace-Amiens/2024-FrontieraApp/assets/158062961/1c843e64-9268-487c-9faf-5bf29b9951f4)  

Cependant nous avons finalement changer d'approche car nous avons rencontrés des problèmes quant à la gestion des réponses. Nous avons donc opter pour une autre méthode.  
Au lieu de créer un tableau pour stocker les questions et les réponses, nous avons créer une base de données avec celles-ci. Lorsque l'utilisateur clique sur une réponse, le programme récupère ainsi l'index de la question et la réponse. Il vérifie s'il s'agit de la bonne, dans ce cas il affiche un panel avec "Bonne Réponse" et dans le cas contraire il affiche l'autre panel avec "Mauvaise Réponse".   
Cette méthode était beaucoup plus facile à gérer et nous permettait en plus de rajouter plus simplement d'autres questions si nécessaire. 

 ![image](https://github.com/Makerspace-Amiens/2024-FrontieraApp/assets/158062961/c773be05-b513-4213-bf61-337e5a02ff20)  

 

 
 
