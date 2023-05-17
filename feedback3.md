# Hello World

---

Comment vas-tu ??? Pas facile cette saison ! Avec beaucoup de notions à assimiler mais tu progresses et ça c'est super à voir !
Tu comprends l'architecture MVC ! 

---

### Routes

Tu as compris le fonctionnement pas de doute mais attention à bien suivre les consignes, ta pages d'accueil n'est pas sur la route indiqué sur le document fournis elle pointe sur /home au lieu de /.

```php
$router->map(
    'GET',
    '/home',
    [
        'method' => 'home',
        'controller' => MainController::class // On indique le FQCN de la classe
    ],
    'main-home'
);
```

Globalement rien à redire tu as compris le fonctionnement des routes en GET et POST et ton ajout en bdd via la methode POST est presque bon!

---

* Petite indication dans ta fonction StudentAdd()  de ton StudendController il manque la gestion de ton "teacher" ;) (la colone teacher_id dans ta bdd).

* Attention au copié collé non corrigé, dans ton teacherController une fonction studentAdd c'est risqué !!!! ;-);

---

Pour assimiler toutes ces nombreuses notions vu cette saison tu peux regarder du coté de Kourou!

les episodes 2 et 3 de cette saison 6 t'aiderons a revoir et pratiquer ces notions 

[https://kourou.oclock.io/ressources/recap-quotidien/nazca-s06e02-backofficeinsert/]
[https://kourou.oclock.io/ressources/recap-quotidien/nazca-s06e03-backofficeupdate/]

N'hésites pas à t'entrainer a refaire les challenges, la pratique il n'y a rien de mieux pour retenir !

