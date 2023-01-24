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

![image](https://user-images.githubusercontent.com/98362303/214358344-0a3a28b4-f09c-4342-9438-efef898d6649.png)

On remarque qu'il y a un bruit qu'on doit éliminer avec un filtrage notch 

3 - Suppression des interférences des lignes électriques 50Hz : 

![image](https://user-images.githubusercontent.com/98362303/214359747-f4ccc73c-85bf-41f7-9fc2-93dd02823720.png)

On remarque que ce signal est encore bruité quand on le compare avec le signal ECG qu'on doit avoir.
Pour eliminer ce bruit on applique un filtrage pass bas pour eliminer les bruits de basses fréquences.

ECG 2 apres le filtrage notch avec ses spectres et le bruit qui doit etre eliminer 

![image](https://user-images.githubusercontent.com/98362303/214360539-afaa8cad-c995-4688-b229-cbf37b9c2ab9.png)


4 - Amélioration du rapport signal sur bruit :

Apres avoir eliminer les filtres on obtient le signal suivant :

![image](https://user-images.githubusercontent.com/98362303/214362201-3c3773b1-c859-4977-8c68-723102160ee8.png)

5 - Identification de la fréquence cardiaque avec la fonction d'autocorrélation :

La fréquence cardiaque peut être identifiée à partir de la fonction d'autocorrélation du signal ECG. Cela se fait en cherchant le premier maximum local après le maximum global (à tau = 0) de cette fonction.

On utilise la fonction xcorr pour le signal ecg3 

![image](https://user-images.githubusercontent.com/98362303/214362925-2c72a219-d38b-4908-8731-4b3a02a13301.png)


On detecte une correlation dans un maximum a taux = 2 


# Réalise par : Khalil Hamdaoui
# Encadré par : Prof Ammour Alae












