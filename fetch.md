 # Fetch

 Fetch est une méthode en JavaScript qui permet de récupérer des informations depuis un serveur distant. Cela peut être des données au format JSON, des images, des fichiers HTML, etc et de les réutiliser.

 par exemple en prenant en compte que tu veux récupérer des informations envoyé par une api en json provenant d'une adresse '/api/teachers'.


 ```JS

fetch('/api/teachers')
  .then(response => response.json())
  .then(data => {
    console.log(data);
  })
  .catch(error => {
    console.error('Une erreur est survenue :', error);
  });

```

Etapes:

1. Tu utilises la méthode Fetch pour demander au serveur des informations à partir de l'URL /api/teachers.
2. Ensuite, tu utilises .then() pour dire au programme quoi faire lorsque le serveur répond. Tu convertis la réponse en format JSON avec response.json().
3. Dans la deuxième partie de .then(), tu peux utiliser les données que tu as reçues. *Dans cet exemple, nous les affichons simplement dans la console avec console.log(data)*.
4. 
5. Si quelque chose ne fonctionne pas et qu'il y a une erreur, tu utilises .catch() pour afficher un message d'erreur.
