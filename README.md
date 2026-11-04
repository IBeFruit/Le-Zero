# Le Zéro

Saloon-casino en dollars fictifs pour jouer entre potes : roulette et blackjack 3D en salons privés, personnage à créer, badges et objets à débloquer.

Site statique (Cloudflare Workers, dossier `public/`) + Firebase (connexion Google et Firestore pour les salons).

## Mise en route
1. Firebase : créer un projet, ajouter une application Web, coller sa configuration dans `public/config.js`.
2. Authentication > Méthode de connexion : activer **Google**. Dans Paramètres > Domaines autorisés, ajouter l'adresse workers.dev du site (et celle de la branche dev).
3. Firestore Database : créer la base (mode production), puis coller le contenu de `firestore.rules` dans l'onglet Règles et publier.
4. Cloudflare : Workers & Pages > projet relié au dépôt ; `wrangler.jsonc` publie le dossier `public/`. Chaque push sur `main` met le site à jour, la branche `dev` donne une adresse d'aperçu.

Jouer en solo marche sans connexion. Les salons demandent un compte Google.
