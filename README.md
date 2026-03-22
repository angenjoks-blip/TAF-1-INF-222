Blog API - INF222 TAF 1

    Description

Ce projet consiste en la création d'une API Backend simple pour la gestion d'un blog, réalisée dans le cadre de l'UE INF222 - Programmation Web. L'apprentissage a été structuré via la plateforme CleeRoute.

    Fonctionnalités
    
L'API permet les opérations suivantes sur les articles :

Créer un article : Titre, contenu, auteur, date, catégorie et tags.

Lire les articles : Récupérer la liste complète ou un article unique par son ID.


Modifier un article : Mettre à jour les informations d'un article existant.

Supprimer un article : Retirer un article de la base de données via son ID.

Recherche : Trouver des articles par un mot-clé dans le titre ou le contenu.

     Technologies Utilisées
     
Langage : Node.js.

Framework : Express.

Base de données : JSON / In-memory (pour ce prototype).

Documentation : Format Swagger (recommandé).

    Installation et Utilisation
    
Cloner le dépôt :

Bash
git clone [LIEN_DE_TON_DEPOT]
Installer les dépendances :

Bash
npm install

Lancer le serveur :

Bash
npm start
Endpoints de l'API
Méthode	Endpoint	Description
POST	/api/articles	
Créer un nouvel article 

GET	/api/articles	
Liste de tous les articles 

GET	/api/articles/:id	
Détails d'un article spécifique 

PUT	/api/articles/:id	
Modifier un article 

DELETE	/api/articles/:id	
Supprimer un article 

GET	/api/articles/search

Codes de Statut HTTP utilisés
200 OK : Requête réussie.

201 Created : Création d'article réussie.

400 Bad Request : Données manquantes ou invalides.

404 Not Found : Article non trouvé.

500 Internal Server Error : Erreur du serveur.
