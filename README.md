# Gestion des absences — Login par rôle (prototype)

Application web React et Vite de démonstration, en français, inspirée des maquettes de calendrier et d'interfaces institutionnelles fournies.

## Lancer le projet

```bash
npm install
npm run dev
```

Pour produire un build : `npm run build`.

## Fonctionnalités

- Connexion de démonstration par identifiant et mot de passe fictif, puis orientation automatique vers les espaces Employé, Manager et Ressources humaines
- Calendrier mensuel et événements colorés par catégorie
- Création de demandes de congés payés, RTT, télétravail, formation et autres absences
- Dates de début et fin, demi-journée sur le premier jour, commentaire libre
- Liste des demandes filtrable par statut
- Historique et commentaires par demande
- Approbation et refus depuis les espaces Manager et RH
- Quatre profils fictifs de démonstration
- Persistance locale dans `localStorage`

## Limites importantes

**Prototype seulement : pas de serveur, d'authentification réelle ni de permissions réelles.** Les changements effectués par un rôle peuvent être vus dans le même navigateur via le sélecteur de profil. Ils ne se synchronisent pas entre appareils ni navigateurs.

Les soldes sont fictifs, la durée ne tient pas compte des jours fériés, et les demi-journées ne s'appliquent qu'au premier jour. Une mise en production nécessite authentification, backend, contrôle des permissions, politique RH, protection des données et conformité RGPD.

## Stack

React 19, Vite 6, Lucide React, CSS responsive.

## Accès à la version Login

Les trois comptes fictifs reconnus sont `emma@demo.fr` (employé), `manager@demo.fr` (manager), et `rh@demo.fr` (RH). Un mot de passe fictif non vide est accepté. Ne saisissez jamais de vrai mot de passe. Le rôle est associé au compte dans le code côté client, et non déterminé par un serveur. Pour une version réelle, le serveur authentifie et fournit le rôle et les autorisations.

Source de cette variante : `axeligato/gestion-des-absences`, branche `prototype/login-by-role`.
