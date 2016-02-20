#Projet BlaBlaCar en J2EE

#Instructions pour lancer le projet : 

1 - Télécharger le projet au format .zip
2 - L'importer dans NetBeans (File -> Import project -> From zip...)
3 - Lancer le main afin de créer les tables de la base de données (BlaBlaCar-ejb -> Source Packages -> main -> TestEjb.java --run file--)
4 - Lancer le projet BlaBlaCar (clic droit -> Deploy) 
  Le projet utilise le serveur GlassFish et la base de données de NetBeans.
5 - Ouvrir le navigateur et se rendre à l'adresse suivante :
  http://localhost:8080/BlaBlaCar-war/accueil.faces

#Travail réalisé
- Il est possible d'ajouter un trajet associé à un utilisateur.
Lorsqu'on ajoute un trajet, le nom et prénom de l'utilisateur sont recherché dans la base pour retrouver l'utilisateur correspondant. S'il n'est pas trouvé, un nouvel utilisateur sera créé.

- Il est possible de rechercher le trajet que l'on vient d'ajouter.

#Exemple

Problème : le système ne fonctionne qu'une seule fois (un seul ajout de trajet possible...)
Lorsque l'on veut ajouter un second trajet, on obtient l'erreur suivante : 
	Error while committing the transaction
	HibernateException: Illegal attempt to associate a collection with two open sessions

#--
D'une façon générale, le système est très capricieux et fonctionne rarement correctement...
En espérant que ça fonctionne au moins une fois chez vous...
