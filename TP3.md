# TP3 Traitement d'un signal ECG

## Objectifs:

Dans ce troisième Tp on cherche a Supprimer du bruit autour
du signal produit par un électrocardiographefaire et faire la
représentation temporelle et fréquentielle en utilisant la
transformée de fourrier discrète sous le logiciel Matlab.

### Introduction : 

Un électrocardiogramme (ECG) est un test qui mesure l'activité électrique du cœur. 
Il est utilisé pour détecter des anomalies cardiaques telles que les troubles du rythme cardiaque,
les infarctus du myocarde et les maladies cardiaques congénitales.



![image](https://user-images.githubusercontent.com/98362303/214177099-07ec047c-6d33-4764-bd16-701e79a66e14.png)

L’onde P représente la première étape du cycle où les oreillettes (ou atriums) se contractent permettant le passage du sang, à travers les valves auriculoventriculaires, vers les ventricules.
Ensuite, le complexe QRS symbolise à la fois la contraction ventriculaire (permettant l’éjection du sang vers les artères) notamment par le pic en R, dans le même temps,le relâchement des oreillettes entraîne le remplissage de celles-ci en attente d’un nouveau cycle).

L’onde T représente le relâchement des ventricules suite à leur contraction.L’enchaînement de ces complexes permet par ailleurs de déterminer la fréquence cardiaque, c’est-à-dire le nombre de cycle cardiaque par unité de temps. Une fréquence cardiaque normale est comprise entre 60 et 100 battements par minute, en dessous de cette valeur, le patient est en « bradycardie », au-dessus de cette valeur,le patient est en « tachycardie ».

Les signaux ECG sont contaminés avec différentes sources de bruits. Les bruits de hautes fréquences sont provoqués par l’activité musculaire extracardiaque et les interférences dues aux appareils électriques, et des bruits de basses fréquences provoqués par les mouvements du corps liés à la respiration, les changements physicochimiques induits par l’électrode posée sur la peau et les micro variations du flux sanguin.
Le filtrage de ces bruits est une étape très importante pour faire un diagnostic réussi.



1 - Suppression du bruit provoqué par les mouvements du corps:

On Sauvegarde le signal ECG sur le répertoire de travail, puis on le charge dans Matlab à l’aide la commande load. Ce signal a été échantillonné avec une fréquence de 500Hz. 
On le trace en fonction du temps, puis on fait un zoom sur une période du signal.

![image](https://user-images.githubusercontent.com/98362303/214177599-44c909fc-4f7a-4620-b7e1-e40120487236.png)

Son spectre d'amplitude :

![image](https://user-images.githubusercontent.com/98362303/214177818-f664f3e9-67fc-4987-8739-b59398b631b0.png)

Ensuite on procède a supprimer le bruit des mouvements du corps en utilisant un filtrage idéal passe haut et on trace la différence par rapport au signal d'origine

![image](https://user-images.githubusercontent.com/98362303/214177949-3959bada-bf77-4e60-a1d6-898d683727e6.png)

2 - Suppression des interférences des lignes électriques 50Hz:

Souvent, l'ECG est contaminé par un bruit du secteur 50 Hz qui doit être supprimé

![image](https://user-images.githubusercontent.com/98362303/214179332-25f97ef2-77ed-4e71-a1fa-b3cb39ddccf6.png)

On remarque qu'il y a un bruit 



















