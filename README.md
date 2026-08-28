# Jemié Hair — Site vitrine + Administration

## Déploiement sur GitHub Pages (compte tikof1980)
1. Crée un dépôt `jemie-hair` sur GitHub.
2. Ajoute les 3 fichiers : `index.html`, `robots.txt`, `sitemap.xml`.
3. Settings → Pages → Source : branche `main`, dossier `/root`.
4. Le site sera disponible à `https://tikof1980.github.io/jemie-hair/`.

## Espace administration
- Lien discret en bas de page : "Espace administration".
- Mot de passe par défaut : `jemie2026` (à changer immédiatement dans Paramètres → Changer le mot de passe).
- Toutes les données (produits, catégories, galerie, témoignages, promotions, textes, coordonnées) sont modifiables sans toucher au code, et sont stockées dans le navigateur (localStorage) de l'appareil utilisé pour l'administration.

## Important à savoir
- **Numéro de téléphone/WhatsApp** : déjà configuré sur `0749444901` (modifiable dans Admin → Contact & Réseaux).
- **Photos** : le site est livré sans photos réelles (aucune image n'a été copiée depuis l'affiche fournie). Ajoute tes propres photos via l'administration pour le portrait d'accueil, les produits, la galerie et l'à-propos — elles sont stockées en base64 dans le navigateur, donc privilégie des images compressées (< 300 Ko) pour rester dans les limites de stockage local.
- **Sécurité** : l'authentification admin est côté client (adaptée à un usage mono-utilisateur sur un site 100% statique). Pour une vraie gestion multi-appareils avec compte sécurisé, il faudra migrer vers une base de données en ligne plus tard (prévu dans l'architecture pour ne pas bloquer cette évolution).
- **Contenu par défaut** : prix, catégories et quelques produits/témoignages d'exemple sont préremplis à partir de la liste "Nos Prestations" — à ajuster dans l'administration selon tes vrais tarifs.

## Stack technique
HTML/CSS/JS pur (fichier unique), JavaScript ES5 compatible Android Chrome, sans framework ni build, `localStorage` pour la persistance, `addEventListener` partout (pas de `onclick` inline).
