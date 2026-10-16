# AI TRADER FACTORY 3.1 — version corrigée

## Publication GitHub Pages
1. Remplace `index.html`, `manifest.webmanifest`, `sw.js` et le dossier `icons/` dans le dépôt.
2. Commit les changements sur la branche publiée (`main`, racine `/`).
3. Recharge le site. Si l'ancien écran reste en cache, ferme l'application installée et recharge dans Chrome.

## Corrections
- Valeur nette = cash disponible + notionnel réservé + P/L brut latent - frais de sortie estimés.
- À la clôture, restitution du notionnel réservé, ajout du P/L brut et déduction des frais de sortie; le P/L réalisé soustrait les deux côtés de frais.
- Contrôle du risque au stop avec estimation des frais d'entrée et de sortie.
- Export CSV et gestionnaire d'export conservés hors de la réinitialisation.
- Mapping des clés de réponse Kraken sur les clés de paires demandées.

## Limites
Paper trading uniquement. Stops contrôlés toutes les ~30 secondes à partir du dernier cours reçu, sans garantie d'exécution au niveau exact. Aucune API privée ni ordre réel. Le score technique n'est pas une probabilité de réussite. Tester les calculs avant tout usage décisionnel.
