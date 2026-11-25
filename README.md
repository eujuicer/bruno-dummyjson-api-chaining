# Bruno — API chaining with DummyJSON

Bruno collection of exercises on pure API request chaining, based on [dummyjson.com](https://dummyjson.com).

## Contents

- **Login** — authentication and token retrieval
- **Utilisateurs** (users) — fetching and creating users
- **Produits** (products) — listing, creating, validations (structure, pagination, 404 errors, mathematical consistency)
- **E-Commerce** — complete user journey in 5 chained requests:
  1. `01 - Login` — authentication, captures `jwt_token` and `user_id`
  2. `02 - Profil Utilisateur` (user profile) — fetches the profile with the token, captures `user_city`
  3. `03 - Panier Utilisateur` (user cart) — fetches the cart, captures `cart_id` and `product_id`
  4. `04 - Détail Produit` (product detail) — fetches the product detail, captures `product_category`
  5. `05 - Produits Similaires` (similar products) — searches for products in the same category

## Usage

Open the folder in [Bruno](https://www.usebruno.com/), select the **Dev** environment, then run the Runner on the `E-Commerce` folder to execute the whole chain.

```bash
npx @usebruno/cli run E-Commerce --env Dev -r
```
