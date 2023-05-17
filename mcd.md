# Alors Les mcd compris ou compris ? ;) 

---

Avant toute chose tu peux jetter un coups d'oeil à la fiche récape de Kourou .

[https://kourou.oclock.io/ressources/fiche-recap/mcd-modele-conceptuel-de-donnees/]

---


Prenons par étapes !

1. Tes entités sont bien dans des rectangles ( ADRESS,ORDER,USER,Product) good job !

2. Les Attributs sont bien listés sous les Entités (exemple email,password) Attention!!! Pas d'id par ici tu peux les retirer c'est un attribu purement technique qui n'a pas sa place dans le mcd!
Autre detail les attributs doivent etre en langue naturel avec des espaces et sans underscore). 

**exemple** = *"postal_code" devient "Code Postal" ;).*

*pssss : ! Tu as une adresse en entité mais une adresse en attributs, peut-être faudrai t'il changé la deuxieme ... une RUE c'est pas mal aussi ;)*

1. Tes associations doivent être représentées par un rectangle arrondi et nommées par un verbe.
il va falloir mettre des rondeurs là dedans ;)  .

1. Concernant les cardinalités petit résumé de Kourou bien util. 
---

**Cardinalités**  :

Les quantités minimum et maximum qui peuvent exister entre deux entités A et B,

de A vers B et de B vers A,

cela implique donc 4 cardinalités par relation, pour les trouver posons-nous ces questions :

**L’entité A** est « liée » à combien **d’entités B** au minimum ? => 0 ou 1

**L’entité A** est « liée » à combien **d’entités B** au maximum ? => 1 ou n

**L’entité B** est « liée » à combien **d’entités A** au minimum ? => 0 ou 1

**L’entité B** est « liée » à combien **d’entités A** au maximum ? => 1 ou n

Partant de là, les valeurs possibles pour les cardinalités sont : (0,1) (1,1) (0,n) (1,n).

**0** = aucune,
**1** = un ou une,
**n** = plusieur.

---
D'aprés ton context un utilisateur peut avoir une adresse au minimum ou plusieur adresse au maximum mais une adresse appartien forcément à un utilisateur et au maximum à un seul utilisateur !


ce qui voudrait dire que ...... l'on serait plus sur du **"ADDRESS 1,1 HAS 1,N USER"** non ? ;) .

Pour corriger ce mcd et les prochains tu peux utiliser [mocodo.net ](https://www.mocodo.net/)
Tres pratique à utiliser avec un peu d'entrainements !

Copie colle ce code dans mocodo tu auras ta relation entre ADRESS et USER Corrigé pour t'indiquer la marche à suivre pour les autres ;) .

```
Adresse: _rue, ville, code postal
Appartiens, 11 Adresse, 1n Utilisateur
Utilisateur: _email, mot de passe
```

---

C'est du bon boulot hein !!!! Et il faut continuer à pratiquer pour s'habituer !!!!
Ne lache rien et n'hésite pas à me partager ta correction quand tu l'auras finie  ;) .
