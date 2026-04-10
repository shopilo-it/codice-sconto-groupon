# Codice sconto Groupon, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Groupon** da [shopilo.it](https://shopilo.it/negozi/groupon.it). Restituisce **coupon Groupon** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-groupon](https://shopilo-it.github.io/codice-sconto-groupon/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-groupon
cd codice-sconto-groupon
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Groupon",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su esperienze e deal locali",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/groupon.it"
  }
]
```

## Coupon Groupon disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 20% | 20% di sconto su esperienze e deal locali | [shopilo.it](https://shopilo.it/negozi/groupon.it) |

Codici attivi: **[shopilo.it/negozi/groupon.it](https://shopilo.it/negozi/groupon.it)**

## Domande frequenti

### Come utilizzo un codice sconto Groupon?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/groupon.it), aggiungi i prodotti al carrello su Groupon e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Groupon?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Groupon piu recenti?
La pagina [shopilo.it/negozi/groupon.it](https://shopilo.it/negozi/groupon.it) viene aggiornata quotidianamente con i codici sconto Groupon, voucher Groupon e coupon promozionali Groupon piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Groupon

Groupon e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/groupon.it) trovi i migliori codici sconto Groupon, coupon Groupon verificati e voucher Groupon attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-groupon
```

```javascript
const { fetchCoupons } = require('codice-sconto-groupon');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
