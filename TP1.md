Dans ce premier Tp on va faire la représentation temporelle
et fréquentielle en utilisant la transformée de fourrier discrète 
sous le logiciel Matlab.
On va ensuite essayer de filtrer idéalement un signal bruité.
(filtre passe-bas)  

N.B : 
- Dans le traitement du signal, la transformée de Fourier 
est utilisée pour analyser et comprendre le contenu en 
fréquence d'un signal.

- Le filtre passe-bas idéal supprime les fréquences supérieures 
à une certaine fréquence de coupure tandis que le filtre 
passe-haut idéal supprime les fréquences inférieures à une 
certaine fréquence de coupure.

![image](https://user-images.githubusercontent.com/98362303/213957224-c57298a3-5595-48db-bdda-c261be2418e0.png)


<?xml version="1.0" encoding="UTF-8"?>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 476 68"/>![image](https://user-images.githubusercontent.com/98362303/213956372-a77199d4-1812-49aa-9216-d8d6a683b8ba.png)

On génére un signal de 5000 échantillons

<?xml version="1.0" encoding="UTF-8"?>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 544.5 200"/>![image](https://user-images.githubusercontent.com/98362303/213956481-01fa10df-3ee3-4c0e-b120-bb6f484b39f0.png)

On applique la TFD qui nous génère un spectre qui est une fonction
complexe qui contient une partie imaginaire et une partie réelle

<?xml version="1.0" encoding="UTF-8"?>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 574.04 130.98"/>![image](https://user-images.githubusercontent.com/98362303/213956781-191b216a-7eb0-4928-92d5-0702866b19c2.png)

On injecte un bruit dans le signal et on affiche les résultats
<?xml version="1.0" encoding="UTF-8"?>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 574 135.96"/>![image](https://user-images.githubusercontent.com/98362303/213956954-bef22c8e-ef9b-4ec7-9ba8-fba3edd6c37b.png)

On intensifie le bruit dans le signal en eugmentant le coefficient
<?xml version="1.0" encoding="UTF-8"?>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 574 211.44"/>![image](https://user-images.githubusercontent.com/98362303/213957053-0708c54f-d62e-46d7-bac9-ceb6c6f1fee8.png)

![image](https://user-images.githubusercontent.com/98362303/213957142-5ddabc72-d49c-4524-9817-3ab8c61d232e.png)



![image](https://user-images.githubusercontent.com/98362303/213957421-ae567fd5-c282-4d59-94f0-251a0aa97cc3.png)

Conception du filtre passe-bas
<?xml version="1.0" encoding="UTF-8"?>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 530.85 196.68"/>![image](https://user-images.githubusercontent.com/98362303/213957465-04072cde-efe8-422d-bf44-ba0137cfa447.png)

Application du filtre
<?xml version="1.0" encoding="UTF-8"?>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 531 173.95"/>![image](https://user-images.githubusercontent.com/98362303/213957484-88287229-41ba-434c-9fa9-a2d6764ca8a6.png)

On peut remarquer que les piques superieur à la
fréquence de coupure ont été éliminés







La difference entre le signal filté et le signal sans le cosinus de frequence 2500
<?xml version="1.0" encoding="UTF-8"?>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 488.7 396.98"/>![image](https://user-images.githubusercontent.com/98362303/213957529-76cee36c-5902-4cb9-b174-356991f165b8.png)


![image](https://user-images.githubusercontent.com/98362303/213957551-352daf14-4738-42fb-ade4-7b0af9392c94.png)


A travers ce premier TP j’ai appris comment représenter des 
signaux et leur TFD, et appliquer un filtrage idéal 

# Réalise par : Khalil Hamdaoui
# Encadré par : Prof Ammour Alae

