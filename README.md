# 🧾 Finly – application web de facturation (Node.js)

Application web pour **gérer ses clients et ses factures** et suivre son activité sur un tableau de bord. Projet full-stack JavaScript côté serveur, avec rendu EJS.

## Fonctionnalités

- Inscription et connexion (mots de passe hachés avec bcrypt, sessions Express, messages flash)
- Gestion des **clients** : création, modification, suppression
- Gestion des **factures** liées à un client : création, modification, suppression, montant, date et statut
- **Tableau de bord** de suivi de l'activité
- Validation des formulaires côté serveur (express-validator)

## Stack

| Couche | Technologies |
|---|---|
| Serveur | Node.js, Express, architecture routes / contrôleurs / modèles |
| Base de données | MongoDB, Mongoose |
| Vues | EJS, Tailwind CSS, daisyUI |

## Lancer le projet

```bash
npm install
# créer un fichier .env avec :
#   MONGODB_URI=mongodb://localhost:27017/finly
#   AUTH_SECRET=une_chaine_secrete
npm run dev        # http://localhost:3000
```

## Structure

```
controllers/   logique métier (clients, factures, utilisateurs, tableau de bord)
libs/models/   schémas Mongoose
routes/        routes Express
views/         pages et composants EJS
```
