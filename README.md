# Codice sconto Mondadori Store, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Mondadori Store** da [shopilo.it](https://shopilo.it/negozi/mondadoristore.it). Restituisce **coupon Mondadori Store** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-mondadori](https://shopilo-it.github.io/codice-sconto-mondadori/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-mondadori
cd codice-sconto-mondadori
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Mondadori Store",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su libri, giochi e multimedia",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/mondadoristore.it"
  }
]
```

## Coupon Mondadori Store disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su libri, giochi e multimedia | [shopilo.it](https://shopilo.it/negozi/mondadoristore.it) |

Codici attivi: **[shopilo.it/negozi/mondadoristore.it](https://shopilo.it/negozi/mondadoristore.it)**

## Domande frequenti

### Come utilizzo un codice sconto Mondadori Store?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/mondadoristore.it), aggiungi i prodotti al carrello su Mondadori Store e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Mondadori Store?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Mondadori Store piu recenti?
La pagina [shopilo.it/negozi/mondadoristore.it](https://shopilo.it/negozi/mondadoristore.it) viene aggiornata quotidianamente con i codici sconto Mondadori Store, voucher Mondadori Store e coupon promozionali Mondadori Store piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Mondadori Store

Mondadori Store e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/mondadoristore.it) trovi i migliori codici sconto Mondadori Store, coupon Mondadori Store verificati e voucher Mondadori Store attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-mondadori
```

```javascript
const { fetchCoupons } = require('codice-sconto-mondadori');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
