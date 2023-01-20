# TP2-Jeux de mots & Synthèse et analyse spectrale d'une gamme de musique
## Objectifs

      1. Comprendre comment manipuler un signal audio avec Matlab, en effectuant certaines opérations classiques sur un fichier audio d’une phrase enregistrée via 
       un smartphone.
      2. Comprendre la notion des sons purs à travers la synthèse et l’analyse spectrale d’une gamme de musique.
  
## Introduction
     Les jeux de mots sont des phrases ou des expressions qui jouent sur les sonorités ou les significations des mots. Dans le domaine de la musique, la synthèse 
     spectrale est une technique utilisée pour créer des sons en combinant différentes fréquences. Cela permet de créer des timbres riches et complexes.
     La synthèse spectrale peut être utilisée pour créer des instruments virtuels ou pour moduler des sons enregistrés. L'analyse spectrale est l'inverse de la 
     synthèse
     spectrale. Il s'agit d'une technique utilisée pour décomposer un son en ses différentes fréquences. Cela permet de comprendre comment un son est créé et de 
     découvrir
     les différentes caractéristiques d'un son.
## Réalisation du TP

#### Partie 1 : Jeux de mots
 
    1-2- Chargement de l'audio et traçage de son signal
    
<img width="790" alt="1" src="https://user-images.githubusercontent.com/86896531/213679138-d6e2b25c-a9ec-46eb-86e4-96797832ef8a.png">
       
    3- Changement de la fréquence d'échantillonage
    
<img width="790" alt="3" src="https://user-images.githubusercontent.com/86896531/213679975-05a25f89-2971-46f2-97e0-177191eeeaf0.png">
       
    4- Traçage du signal en fonction des  indices du vecteur x 
            • Le segment "Rien ne sert de" commence de 1 à 75000

<img width="788" alt="4" src="https://user-images.githubusercontent.com/86896531/213680616-c4d081cb-d8b4-4ae8-824c-0ad6794d7d3a.png">
       
    5- Segmenter les premier mot et écouter le
<img width="788" alt="5" src="https://user-images.githubusercontent.com/86896531/213682419-3e6c8688-2bec-42ba-a9c9-8d3775ac7ad0.png">
       
    6- Segmenter toute la phrase
<img width="788" alt="6" src="https://user-images.githubusercontent.com/86896531/213683410-970b2b68-912b-43f0-8761-ecf4bee3b42d.png">
       
    7- Notez que le signal initial de parole est un vecteur colonne contenant un certain nombre de valeurs (length(x)). Réarrangez ce vecteur 
<img width="788" alt="7" src="https://user-images.githubusercontent.com/86896531/213684239-1014f07d-f831-4d26-854e-939db9d465ba.png">

#### Partie 2 : Synthèse et analyse spectrale d’une gamme de musique
 
    2.1: Synthèse d’une gamme de musique 
       1- Créez un programme qui permet de jouer une gamme de musique
 <img width="790" alt="2 1" src="https://user-images.githubusercontent.com/86896531/213686744-86bf3de3-25ba-424a-8fbf-dcb03e0e0977.png">

    2.2: Spectre de la gamme de musique

       2- Visualisation du spectre de la gamme en utilisant l’outil graphique d’analyse de signaux **signalAnalyzer**

         • Signal Analyzer est un outil logiciel développé par MathWorks, utilisé pour l'analyse de signaux numériques. Il permet de visualiser, de mesurer et de
         déboguer des signaux numériques en utilisant des techniques d'analyse tels que l'analyse temporelle, l'analyse fréquentielle et l'analyse de spectre. Il
         offre une interface graphique intuitive pour l'analyse de signaux en temps réel et enregistrés, ainsi qu'un grand nombre de fonctionnalités avancées pour
         l'analyse de signaux complexes.
 <img width="904" alt="2 2" src="https://user-images.githubusercontent.com/86896531/213687154-1738dcf5-513c-48da-8148-345e14c3528b.png">

       3- Traçage du spectrogramme

         • Un spectrogramme est un type de graphique utilisé pour visualiser la répartition de l'énergie d'un signal dans le temps et dans le domaine fréquentiel. 
         Ilest généralement utilisé pour étudier les signaux audio et les signaux de communication. Il est produit en utilisant une technique d'analyse appelée
         analyse
         spectrale en temps-fréquence.
         • Un spectrogramme est généralement représenté sous forme d'image, avec l'axe des x représentant le temps, l'axe des y représentant la fréquence, et la 
         couleur ou la luminosité représentant l'intensité de l'énergie à chaque point de temps et de fréquence. Les couleurs les plus foncées dans un spectrogramme
         indiquent une plus grande intensité d'énergie à une fréquence donnée à un moment donné, tandis que les couleurs plus claires indiquent une plus faible
         intensité d'énergie. Les spectrogrammes sont utilisés pour identifier les caractéristiques de fréquence d'un signal, comme les formants dans la parole,
         les harmoniques dans les instruments de musique, et les signaux cachés dans les bruits de fond.
 <img width="841" alt="2 3" src="https://user-images.githubusercontent.com/86896531/213687469-fcad08b4-caf6-4ff9-b730-4f5ff0654a30.png">

    2.3:  Approximation du spectre d’un signal sinusoïdal à temps continu par FFT

       4- Spectre de fréquence de la gamme musicale crée en échelle linéaire, puis avec une échelle en décibels.
        • L'échelle linéaire est utilisée pour mesurer des valeurs proportionnelles les unes aux autres, tandis que l'échelle en décibels est utilisée pour mesurer
          des niveaux de puissance ou de son qui varient sur des plages très grandes. L'échelle en décibels est un logarithme de l'échelle linéaire, ce qui permet  
          de représenter des valeurs de manière plus compacte.
 <img width="945" alt="2 4 1" src="https://user-images.githubusercontent.com/86896531/213690193-aa4fe157-ee5e-42f9-b1ad-e7243a4db197.png">
 <img width="944" alt="2 4 2" src="https://user-images.githubusercontent.com/86896531/213690228-f98d8fa1-ed03-4f8a-8ce6-869ff81338c2.png">

        
## Conclusions
    En résumé, la synthèse et analyse spectrale sont des outils utilisés pour créer et étudier les sons en utilisant la répartition de l'énergie dans le domaine
    fréquentiel. Les jeux de mots, quant à eux, sont des phrases qui jouent sur les sonorités ou les significations des mots. Il n'y a pas de lien direct entre les
    deux.
