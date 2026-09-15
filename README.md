# Bruno — Chaînage d'API avec DummyJSON

Collection Bruno d'exercices sur le chaînage pur de requêtes API, basée sur [dummyjson.com](https://dummyjson.com).

## Contenu

- **Login** — authentification et récupération de token
- **Utilisateurs** — consultation et création d'utilisateurs
- **Produits** — listing, ajout, validations (structure, pagination, erreurs 404, cohérence mathématique)
- **E-Commerce** — parcours utilisateur complet en 5 requêtes chaînées :
  1. `01 - Login` — authentification, capture de `jwt_token` et `user_id`
  2. `02 - Profil Utilisateur` — récupération du profil via le token, capture de `user_city`
  3. `03 - Panier Utilisateur` — récupération du panier, capture de `cart_id` et `product_id`
  4. `04 - Détail Produit` — détail du produit, capture de `product_category`
  5. `05 - Produits Similaires` — recherche des produits de la même catégorie

## Utilisation

Ouvrir le dossier dans [Bruno](https://www.usebruno.com/), sélectionner l'environnement **Dev**, puis lancer le Runner sur le dossier `E-Commerce` pour exécuter la chaîne complète.

```bash
npx @usebruno/cli run E-Commerce --env Dev -r
```
