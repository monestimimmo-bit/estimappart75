# EstimAppart75 — guide de migration avant publication

Cette archive est une copie préparée du site statique HTML/CSS/JavaScript. Elle ne modifie pas le dépôt GitHub.

## Modifications apportées
- Remplacement de l'identité visible et des données structurées par **EstimAppart75**.
- Remplacement des URL canoniques, Open Graph, sitemap et robots.txt par `https://estimappart75.fr`.
- Nouveau contenu d'accueil et de présentation axé sur la mise en relation de particuliers ayant un projet de vente avec un conseiller immobilier.
- Clarification du parcours : formulaire de demande, prise de contact, rendez-vous et visite du logement par le conseiller.
- Réécriture de l'article auparavant consacré à la comparaison avec l'estimation en ligne, sans changer son nom de fichier afin de préserver son URL.
- Conservation des fichiers CSS, JavaScript, images et des fonctionnalités existantes, sauf les ajustements textuels nécessaires.
- Conservation de l'identifiant GA4 `G-2FR1WCRT6G` et de l'action Formspree existante.

## À faire avant de publier
1. Acheter `estimappart75.fr`.
2. Dans les paramètres GitHub Pages du dépôt, définir `estimappart75.fr` comme domaine personnalisé. Le fichier `CNAME` de cette archive contient déjà ce nom.
3. Configurer les DNS du nouveau domaine selon les instructions GitHub Pages de ton registrar, puis activer HTTPS dans GitHub Pages.
4. Tester toutes les pages, les formulaires et le bandeau de consentement aux cookies après le déploiement.
5. Mettre en place séparément les redirections HTTP 301 de chaque URL de l'ancien domaine vers son équivalent sur `estimappart75.fr`. GitHub Pages ne fournit pas de règles serveur génériques de redirection pour un ancien domaine.
6. Dans GA4, conserver la propriété et l'identifiant de mesure existants, mais mettre à jour l'URL du flux Web.
7. Ajouter et vérifier `estimappart75.fr` dans Google Search Console, envoyer `https://estimappart75.fr/sitemap.xml`, puis utiliser l'outil de changement d'adresse de l'ancienne propriété une fois les redirections opérationnelles.
8. Mettre à jour les liens externes que tu contrôles (fiche établissement, réseaux sociaux, annuaires, signatures e-mail).

## Vérifications et points d'attention
- Les 31 pages HTML possèdent une URL canonique sur le nouveau domaine.
- Les 30 URL du sitemap utilisent le nouveau domaine. La page des mentions légales reste exclue du sitemap, comme dans le site source.
- Les données structurées JSON-LD ont été analysées : aucune erreur de syntaxe détectée.
- Les liens internes locaux ont été vérifiés : aucune cible de fichier manquante détectée.
- L'identifiant GA4 et l'endpoint Formspree existants ont été conservés.

### Mentions légales à compléter impérativement
Le fichier `mentions-legales.html` d'origine contient encore des champs entre crochets : identité et coordonnées de l'éditeur, SIRET, directeur de publication, rémunération, informations sur les partenaires, adresse de contact et durée de conservation des données. Ces informations ne doivent pas être inventées. Complète-les et vérifie la conformité juridique avant mise en ligne.

### Formulaire et données personnelles
Le formulaire transmet des informations personnelles à l'endpoint Formspree existant. Vérifie que le service, les destinataires effectifs, la notice d'information et le consentement correspondent toujours à ton fonctionnement réel et à tes accords avec les conseillers partenaires.

### Nom des fichiers
Le fichier `estimation-en-ligne-ou-avec-un-conseiller.html` garde volontairement son nom actuel pour ne pas changer son URL historique. Son titre, son contenu visible et ses données structurées ont été réécrits pour correspondre au positionnement EstimAppart75. Aucun ancien nom de marque ni ancien domaine n'est conservé dans le contenu textuel du site livré.
