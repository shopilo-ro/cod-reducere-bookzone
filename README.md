# Cod reducere Bookzone — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Bookzone** de pe [shopilo.ro](https://shopilo.ro/magazin/bookzone.ro). Returneaza **cupoane Bookzone** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-bookzone](https://shopilo-ro.github.io/cod-reducere-bookzone/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-bookzone
cd cod-reducere-bookzone
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Bookzone",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% EXTRA la toate cartile",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/bookzone.ro"
  }
]
```

## Cupoane Bookzone disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 20% | 20% EXTRA la toate cartile | [shopilo.ro](https://shopilo.ro/magazin/bookzone.ro) |

Codurile active: **[shopilo.ro/magazin/bookzone.ro](https://shopilo.ro/magazin/bookzone.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Bookzone?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/bookzone.ro), adauga produsele in cos pe Bookzone, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Bookzone?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Bookzone?
Pagina [shopilo.ro/magazin/bookzone.ro](https://shopilo.ro/magazin/bookzone.ro) este actualizata zilnic cu cele mai noi cod reducere Bookzone, voucher Bookzone si cupon promotional Bookzone.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Bookzone

Bookzone este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/bookzone.ro) cele mai bune cod reducere Bookzone, cupoane Bookzone verificate si voucher Bookzone active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-bookzone
```

```javascript
const { fetchCoupons } = require('cod-reducere-bookzone');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
