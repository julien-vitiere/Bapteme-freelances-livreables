# Hello World

---

Comment vas-tu ? 😊 Pas facile cette saison ! Avec beaucoup de notions à assimiler, mais tu progresses et ça, c'est super à voir ! Tu comprends l'architecture MVC !

## Routes

Tu as bien compris le fonctionnement, pas de doute là-dessus, mais attention à bien suivre les consignes. Ta page d'accueil ne correspond pas à la route indiquée dans le document fourni. Elle pointe vers `/home` au lieu de `/`.

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


---

**Globalement, rien à redire.** Tu as bien compris le fonctionnement des routes en GET et POST, et ton ajout en base de données via la méthode POST est presque bon !

Quelques indications:

- Petite indication dans la fonction `StudentAdd()` de ton `StudentController`: il manque la gestion du champ "teacher" 😉 (la colonne `teacher_id` dans ta base de données).
- Attention au copié-collé non corrigé dans ton `TeacherController`: une fonction `studentAdd` est risquée !!!! 😅

Ressources supplémentaires:

Pour assimiler toutes ces nombreuses notions vues cette saison, tu peux regarder du côté de **Kourou**! Les épisodes 2 et 3 de cette saison 6 t'aideront à revoir et pratiquer ces notions:

- [Épisode 2 - Backoffice Insert](lien_vers_l'épisode_2)
- [Épisode 3 - Backoffice Update](lien_vers_l'épisode_3)

N'hésite pas à t'entraîner à refaire les challenges. La pratique est le meilleur moyen de retenir!

---