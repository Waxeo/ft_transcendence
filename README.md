# Transcendance

## GIT USE

Creer sa branche : **git branch nom_de_la_branche**

Move vers la nouvelle branche : **git checkout nom_de_la_branche**

En une commande : **git checkout -b nom_de_la_branche**

Pousser nouvelle branche local avec branche distante : **git push -u origin nom_de_la_branche**

Vous pouvez maintenant faire ce que vous voulez depuis votre branche. Une fois la fonctionnalité terminée, vous pouvez check les modifications depuis github.
Une fois tout bon : 

>[!CAUTION]
>**Ne pas oublier de push sur sa branch avant !**

Retourner sur le main : **git checkout main**

Fusionner les branch : **git merge nom_de_la_branche**

Regler les conflits (par defaut) : **git config pull.rebase false**

>[!TIP]
>Le commit pointe deja vers celui qui vient de merge, plus qu'a **git push**.

>[!NOTE]
>Pour modifier des commentaires, le README ou toutes autres modif ne risquant pas de tout casser, faites le depuis le **main**.

Pour mettre a jour votre branche par rapport au main : **git pull origin main**

## DEV USE

Pour un acces classique : **make**

Pour un acces avec visualisation de bdd : **make dev**

Acces bdd avec make dev : **http://localhost:5000**

Login pgadmin : **admin@admin.com**

MDP admin : **root**

Acceder a la page d'accueil via : **https://localhost:3000**

Nettoyer tout les docker : **./clear.sh**

### PGADMIN4

Pgadmin est une interface graphique pour postgresql. Vous pourrez donc avoir une vision generale de votre db sans vous connecter au docker de la db et s'emmerder avec des commandes SQL

Pour se connecter : 
- **login** = admin@admin.com
- **mdp** = root

Une fois connecter derouler l'arbre de **Servers**

Si il n'y que **Database** qui apparait (ce qui sera surement le cas), faites un clic droit sur **Servers** -> **Nouveau** -> **Serveur**

Une page de config s'ouvre. Dans **General** -> **Nom**, choisissez un nom.

Aller dans **Connexion** : 
- **Nom d'hote** = db
- **Port** = 5432
- **Nom utilisateur** = theuser
- **Mot de passe** = abc

Vous avez maintenant acces a la db sous le nom que vous lui avez donne. C'est un beau bordel alors on va surtout s'interresser au Tables de le db.

Pour y acceder : **Base de donnees** -> **mydb** -> **Schemas** -> **public** -> **Tables**

Tous les modeles que nous allons creer via Django seront visible de la.




## ROADMAP 

### FRONTEND

### BACKEND

## MODULE LIST

### MAJEUR

- [x] Backend Django
- [ ] Gestion utilisateur standard (WIP)
- [x] Authentification a distance
- [x] 2FA (TODO)
- [x] 3D
- [x] BOT 

### MINEUR

- [x] BDD Postgre
- [x] Frontend Bootstrap

### TOTAL POINTS

6 **/ 7**