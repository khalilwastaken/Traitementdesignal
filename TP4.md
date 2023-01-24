# TP4 Filtrage analogique 


## Objectifs :
- Appliquer un filtre réel pour supprimer les composantes indésirables d’un signal.
- Améliorer la qualité de filtrage en augmentant l’ordre du filtre.

## Introduction :

Le filtrage analogique est une technique utilisée pour séparer les différentes fréquences d'un signal analogique en utilisant des composants électroniques tels que des résistances, des condensateurs et des inducteurs. Il existe différents types de filtres analogiques, notamment les filtres passe-bas, passe-haut, passe-bande et coupure de bande, chacun ayant des caractéristiques de fréquence de coupure et de pente différentes. Les filtres analogiques sont utilisés dans une variété d'applications, telles que la radio, la télévision, la communication, les équipements audio et les instruments de mesure.

### 1 - Filtrage et diagramme de Bode : 

![image](https://user-images.githubusercontent.com/98362303/214366581-2451c7ce-9d78-43dd-89a4-2599fd869018.png)


On Trace le signal x(t) et sa transformé de Fourrier

![image](https://user-images.githubusercontent.com/98362303/214366674-7c204fa2-ca66-430d-b6c3-f0a534c2fc27.png)



La transmittance complexe est un concept utilisé pour décrire la performance d'un filtre analogique ou d'un autre système de traitement de signal. Elle est définie comme le rapport entre la tension de sortie d'un système et la tension d'entrée, exprimé en tant que nombre complexe. La transmittance complexe est généralement exprimée en fonction de la fréquence, et elle peut être représentée graphiquement sur un diagramme de Bode, qui montre la fréquence en abscisse et la transmittance complexe en ordonnée. La transmittance complexe peut être utilisée pour déterminer les caractéristiques de fréquence d'un système, telles que les fréquences de coupure et la pente, ainsi que pour concevoir et optimiser les filtres et les autres systèmes de traitement de signal.

![image](https://user-images.githubusercontent.com/98362303/214366970-f0ed0fc4-3cf2-47a6-94ca-47a285e85120.png)

On trace le module de H, son gain et son déphasage avec T=0.0005

![image](https://user-images.githubusercontent.com/98362303/214367263-9ab4ae6a-3803-49f3-a475-7e27c2192494.png)


On applique sur le signal la transmittance complexe de frequence 1000

![image](https://user-images.githubusercontent.com/98362303/214369937-a437a229-3816-4ea9-ae1a-8e74ecab66f1.png)

On remarque que les filtres analogiques sont moins efficaces que les filtres réels, on ne peut pas eliminer les bruits de basses frequances complétement, on pourra juste les diminuer.



### 2 - Dé-bruitage d'un signal sonore

Dans son petit studio du CROUS, un mauvais futur ingénieur a enregistré une
musique en « .wav » avec un très vieux micro. Le résultat est peu concluant, un bruit
strident s'est ajouté à sa musique. Heureusement son voisin, expert en traitement du
signal est là pour le secourir : 

« C'est un bruit très haute fréquence, il suffit de le supprimer. » dit-il sûr de lui.


On trace le signal et sa transformée de fourrier : 

![image](https://user-images.githubusercontent.com/98362303/214373056-5d9c42dc-db2c-4269-b1a2-e734f7ed5d22.png)

On remarque que dans le spectre suivant il y a une fréquence entre 4000 et 6000 d'amplitude 2 qui constitue le bruit, pour l'éiminer on doit appliquer un 
filtre passe bas qui nous permettra de diminuer l'intensité du bruit.

On utilise un filtre butterworth d'ordre 100 : 

Spectre du signal apres l'application du filtre : 

![image](https://user-images.githubusercontent.com/98362303/214372929-a7b3145e-2179-4064-87db-2c1f996650de.png)


On remarque qu'on a pu éliminer le bruit.

















# Réalise par : Khalil Hamdaoui
# Encadré par : Prof Ammour Alae
