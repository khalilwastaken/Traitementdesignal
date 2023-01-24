# TP 2 Jeux de mots / Synthèse et analyse spectrale d’une gamme de musique 

## Objectifs du TP : 
Lors de ce TP on cherche a comprendre comment manipuler un signal audio avec Matlab, en effectuant certaines opérations classiques sur un fichier audio d’une phrase enregistrée via un smartphone. 
On essaye aussi de comprendre la notion des sons purs à travers la synthèse et l’analyse spectrale d’une gamme de musique.

## Introduction : 

le traitement du signal se réfère à la manipulation des signaux audio pour obtenir un effet spécifique. Cela peut inclure l'amplification, la suppression du bruit, l'égalisation, la compression, la réverbération et d'autres effets pour améliorer ou modifier le son. Le but du traitement du signal est de modifier le son pour obtenir un résultat souhaité, comme une meilleure qualité d'écoute ou une ambiance sonore particulière. Les deux domaines travaillent ensemble pour créer un environnement d'écoute optimal.


### 1 - Jeux de mots : 

« phrase.wave » est un fichier audio enregistré à l’aide d’un smartphone, en prononçant lentement la phrase :

- « Rien ne sert de courir, il faut partir à point »

Apres avoir Sauvegarder le fichier sur le répertoire de travail, puis l'avoir dans MATLAB à l’aide de la commande « audioread », On trace le signal le signal enregistré 
et on l'ecoute en utilisant la commande sound

![image](https://user-images.githubusercontent.com/98362303/214173077-65429b1d-070f-41d8-a20a-49d9ab17a069.png)

Densité spectrale du signal : 

![image](https://user-images.githubusercontent.com/98362303/214173995-a9a6c456-a41d-4706-8763-9f5233a3041f.png)

Donald Duck (audio compressé) 
Terminator (audio dilaté)

![image](https://user-images.githubusercontent.com/98362303/214174142-1be610ce-2c96-4cd3-b1ea-844d2b2f1e06.png)

 On trace le signal en fonction des indices du vecteur x, puis on essaye de repérer les indices de début et de fin de la phrase « Rien ne sert de ».

![image](https://user-images.githubusercontent.com/98362303/214174519-77ca30b8-01c5-4bd0-bb9b-f19773bc8838.png)

On segmente les autres parties de la phrase puis on les arrange 

![image](https://user-images.githubusercontent.com/98362303/214174703-aeafe23e-fda6-4fb4-8ed6-bbae6fb0bb55.png)


### 2 - Synthèse et analyse spectrale d’une gamme de musique : 


- Synthèse d’une gamme de musique

Les notes de musique produites par un piano peuvent être synthétisées approximativement numériquement. En effet, chaque note peut être considérée comme 
étant un son pur produit par un signal sinusoïdal. La fréquence de la note « La » est par exemple de 440 Hz.

![image](https://user-images.githubusercontent.com/98362303/214175341-6e6eddf2-0d7a-4d06-b98d-a5c9c0bf8524.png)

- Spectre de la gamme de musique

![image](https://user-images.githubusercontent.com/98362303/214176141-94532747-90e8-415b-9310-9c504e73e1f1.png)

- Approximation du spectre d’un signal sinusoïdal à temps continu par FFT

![image](https://user-images.githubusercontent.com/98362303/214176159-1d8bd176-fa08-407c-ba06-a447159d77c6.png)



# Réalise par : Khalil Hamdaoui
# Encadré par : Prof Ammour Alae



