# Cod reducere Groupon — fetch automat de pe shopilo.it

Modul Python pentru fetch automat de **coduri de reducere Groupon** de pe [shopilo.it](https://shopilo.it/magazin/groupon.it). Returneaza **cupoane Groupon** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-it.github.io/codice-sconto-groupon](https://shopilo-it.github.io/codice-sconto-groupon/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-groupon
cd codice-sconto-groupon
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Groupon",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su esperienze e deal locali",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/magazin/groupon.it"
  }
]
```

## Cupoane Groupon disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 20% | 20% di sconto su esperienze e deal locali | [shopilo.it](https://shopilo.it/magazin/groupon.it) |

Codurile active: **[shopilo.it/magazin/groupon.it](https://shopilo.it/magazin/groupon.it)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Groupon?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.it](https://shopilo.it/magazin/groupon.it), adauga produsele in cos pe Groupon, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Groupon?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Groupon?
Pagina [shopilo.it/magazin/groupon.it](https://shopilo.it/magazin/groupon.it) este actualizata zilnic cu cele mai noi cod reducere Groupon, voucher Groupon si cupon promotional Groupon.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Groupon

Groupon este unul dintre magazinele online populare. Gasesti pe [shopilo.it](https://shopilo.it/magazin/groupon.it) cele mai bune cod reducere Groupon, cupoane Groupon verificate si voucher Groupon active, actualizate zilnic.

## Instalare npm

```bash
npm install codice-sconto-groupon
```

```javascript
const { fetchCoupons } = require('codice-sconto-groupon');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.it](https://shopilo.it)
