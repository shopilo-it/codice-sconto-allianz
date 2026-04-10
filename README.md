# Codice sconto Allianz, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Allianz** da [shopilo.it](https://shopilo.it/negozi/allianz.it). Restituisce **coupon Allianz** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-allianz](https://shopilo-it.github.io/codice-sconto-allianz/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-allianz
cd codice-sconto-allianz
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Allianz",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su polizze auto e casa",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/allianz.it"
  }
]
```

## Coupon Allianz disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su polizze auto e casa | [shopilo.it](https://shopilo.it/negozi/allianz.it) |

Codici attivi: **[shopilo.it/negozi/allianz.it](https://shopilo.it/negozi/allianz.it)**

## Domande frequenti

### Come utilizzo un codice sconto Allianz?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/allianz.it), aggiungi i prodotti al carrello su Allianz e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Allianz?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Allianz piu recenti?
La pagina [shopilo.it/negozi/allianz.it](https://shopilo.it/negozi/allianz.it) viene aggiornata quotidianamente con i codici sconto Allianz, voucher Allianz e coupon promozionali Allianz piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Allianz

Allianz e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/allianz.it) trovi i migliori codici sconto Allianz, coupon Allianz verificati e voucher Allianz attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-allianz
```

```javascript
const { fetchCoupons } = require('codice-sconto-allianz');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
