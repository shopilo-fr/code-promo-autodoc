# Code promo Autodoc, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Autodoc** depuis [shopilo.fr](https://shopilo.fr/reductions/auto-doc.fr). Renvoie les **coupons Autodoc** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-autodoc](https://shopilo-fr.github.io/code-promo-autodoc/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-autodoc
cd code-promo-autodoc
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Autodoc",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur les pieces auto",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/auto-doc.fr"
  }
]
```

## Coupons Autodoc disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur les pieces auto | [shopilo.fr](https://shopilo.fr/reductions/auto-doc.fr) |

Codes actifs : **[shopilo.fr/reductions/auto-doc.fr](https://shopilo.fr/reductions/auto-doc.fr)**

## Questions frequentes

### Comment utiliser un code promo Autodoc ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/auto-doc.fr), ajoutez les produits a votre panier sur Autodoc et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Autodoc ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Autodoc les plus recents ?
La page [shopilo.fr/reductions/auto-doc.fr](https://shopilo.fr/reductions/auto-doc.fr) est mise a jour quotidiennement avec les codes promo Autodoc, bons de reduction Autodoc et coupons promotionnels Autodoc les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Autodoc

Autodoc est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/auto-doc.fr), retrouvez les meilleurs codes promo Autodoc, coupons Autodoc verifies et bons de reduction Autodoc actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-autodoc
```

```javascript
const { fetchCoupons } = require('code-promo-autodoc');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
