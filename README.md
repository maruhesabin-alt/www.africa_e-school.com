# AFRICA E-SCHOOL V3

Site de formations en ligne (HTML, CSS et JavaScript natifs, sans dépendance).

## Lancer
1. Ouvrez le dossier dans VS Code, clic droit sur `index.html`, « Open with Live Server ».
2. Administration : bouton en haut à droite. Code dans `CONFIG.adminPin` (à changer).

## Contenu
- `index.html` : application complète (pages Accueil, Formations, Détail, Lecteur, FAQ, Administration, Aperçu).
- `images/f1.svg` … `f15.svg` : illustrations vectorielles créées pour le projet (une par formation). `images/maquette-promo.png` : maquette de référence, non affichée.
- `logo.png` : logo.
- `docs/` : configuration, déploiement, paiement, rapport de tests, liens à vérifier.
- `.env.example` : variables du futur serveur (aucun secret réel).

## Ce que la V3 fait vraiment
Navigation avec bouton Retour et fil d’Ariane, catalogue (recherche, filtres, tri), page de détail, lecteur avec leçons précédente/suivante, progression et reprise, aperçu ordinateur/tablette/téléphone, administration locale, animations avec respect de « réduire les animations ».

## Ce que la V3 ne fait pas encore (nécessite un serveur)
Comptes avec mot de passe, vérification d’e-mail, droits d’accès vérifiés côté serveur, administration protégée côté serveur, avis modérés, paiement AvadaPay. Les données (catalogue modifié, progression, notes) sont stockées dans le navigateur de chaque appareil. Voir `docs/DEPLOIEMENT.md`.

## V3.1 — corrections lecteur et navigation
- Lecteur vidéo intégré agrandi et responsive, mode cinéma, plein écran, liste de leçons réductible et recherche dans les leçons.
- Les leçons individuelles sont interactives; la progression est conservée sur l'appareil.
- Les dossiers Google Drive nécessitent des liens individuels de vidéo dans l'administration tant que l'API Drive côté serveur n'est pas configurée.
- La recherche catalogue couvre les titres, catégories, descriptions et mots-clés et peut être effacée rapidement.
- Lire `docs/RAPPORT-DE-TESTS.md` avant la mise en production : les comptes, les droits côté serveur, les paiements et la protection réelle des cours ne sont pas encore configurés.
