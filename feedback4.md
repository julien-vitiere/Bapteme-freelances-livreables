# Hey ! Alors, cette saison ? Sportive hein !
---

Alors, alors !!!
Trop vite est l'ennemi du bien ! Tu as compris pas mal de notions mais tu sembles t'être éparpillé dans ce parcourt !

Reprenons par étapes ;-).

---
### La méthodologie MVC.

MVC (Modèle-Vue-Contrôleur) est une méthodologie utilisée pour structurer et organiser les applications web. Elle divise une application en trois composants principaux :

Modèle : Le modèle représente les données de l'application et gère leur manipulation. Il est responsable de l'accès aux données, des opérations de lecture/écriture dans la base de données et de la logique métier associée.

  ***Exemple: Teachers dans ton code***

Vue : La vue est responsable de l'affichage des données et de l'interface utilisateur. Elle reçoit les données du contrôleur et les présente de manière appropriée aux utilisateurs. Elle peut être une page HTML, un fichier XML, un fichier PDF, etc.

***exemple: teachers_list.tpl.php dans ton code***

Contrôleur : Le contrôleur agit comme un intermédiaire entre le modèle et la vue. Il reçoit les requêtes de l'utilisateur, effectue les actions nécessaires et détermine quelle vue doit être affichée. Il récupère les données du modèle, les prépare et les envoie à la vue pour affichage.

***Exemple: TeachersController dans ton code***

---

Dans ton code tu as voulu aller trop vite !

Il faut reprendre la correction et le faire tranquillement ! Ca va bien se passer :-D !

Il te manque deux controllers importants pour que ton code fonctionne .

Ton MainController n'existe pas dans tes controllers !!!
et ton CoreController qui contient tout ce code répétitif que tu as "*extends*" n'existe pas non plus .
Sans les fondations de ta maison, tout s'écroule !

Une fois que tu auras repris ces deux elements importants on peut continuer !

Dans ta fonction teachers (dans ton TeachersController),
tu dois faire appel à la méthode "static" de la classe Teachers.

En modifiant un tout petit peu ton code on serait plutot dans ce genre là 

```php
public function teachers() {

        
        $teachers = Teacher::findAll();

        $this->show("teachers/teachers_list", [
            'teachers' => $teachers
        ]);
        
    }
```
Et a ce moment là tu pourras passer à l'affichage sur ton fichier *teachers_list.tpl.php*
.

Pour la suite tu sembles avoir compris une bonne partie pour les ajouts et modifications, avec l'aide de la correction tu devrais façilement avancer ! Courage !
Tu peux reprendre les notions via kourou aprés un peu de repos mérité sur cette saison quand même !

Par ici tu auras un rappel sur les héritages et les methodes statics
[https://kourou.oclock.io/ressources/fiche-recap/heritage/]

N'hesite pas à faire fonctionner l'entraide en cas de doute dans ta correction ou à revenir vers nous!

Si il te reste du temps et de l'énergie tu peux en profiter pour refaire les challenges de cette saison en les améliorant ! La pratique c'est là meilleur façon de retenir !