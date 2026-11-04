# Le Zéro

Saloon-casino en dollars fictifs pour jouer entre potes : roulette et blackjack 3D en salons privés, personnage à créer, badges et objets à débloquer.

Site statique (GitHub Pages) + Firebase (connexion Google et Firestore pour les salons).

## Mise en route
1. Firebase : créer un projet, ajouter une application Web, coller sa configuration dans `config.js`.
2. Authentication > Méthode de connexion : activer **Google**. Dans Paramètres > Domaines autorisés, ajouter `ibefruit.github.io`.
3. Firestore Database : créer la base (mode production), puis coller le contenu de `firestore.rules` dans l'onglet Règles et publier.
4. GitHub : Settings > Pages > Deploy from a branch > `main` / racine.

Jouer en solo marche sans connexion. Les salons demandent un compte Google.
