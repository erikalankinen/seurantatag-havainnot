# Seurantatagien havainnointiohjelmat
Tämä projekti on osa kandidaatin tutkielmaa, jossa käsitellään seurantatageista kerättyä havaintodataa. Sovellus lukee, käsittelee ja analysoi havaintoja tutkimuskäyttöön.

Repository sisältää kaksi Python-ohjelmaa seurantatagien havainnointiin:
- `tile.py` seuraa Tile-laitetta (pytile-kirjastolla)
- `samsung.py` seuraa Galaxy Tag 2 -laitetta (SmartThings API)

## Asennus  
```bash 
pip install aiohttp pytile requests
```

## Käyttö
- Tile: lisää tiedostoon EMAIL ja PASSWORD placeholderien tilalle. Suorita `python tile.py`. Havainnot tallentuvat `tile_havainnot.csv`.
- Samsung: lisää tiedostoon PAT placeholderin tilalle. Suorita `python samsung.py`. Havainnot tallentuvat `samsung_havainnot.csv`.

## Huomio
- AirTagin ja MotoTagin havainnot eivät ole ohjelmallisesti saatavilla.
- Samsung koodia ei ole täysin testattu eikä se ehkä toimi kaikissa ympäristöissä.
