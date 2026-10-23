# HESSU 64 – Softa

Retrohenkinen selaimessa toimiva "portfoliopääte" ja ohjelmisto-launcher. Projekti on rakennettu yhden HTML-tiedoston ympärille ja simuloituna 8-bittisen tietokoneen komentorivinäyttönä.

## Kuvaus

Tämä sivu toimii kuin "HESSU 64" -niminen käyttöliittymä, jossa käyttäjä voi:

- listata ohjelmia ja projekteja
- käyttää komentoja kuten `HELP`, `DIR`, `LOAD`, `ABOUT`, `GITHUB`
- siirtyä suoraan GitHubiin tai muihin projektisivuihin
- tutustua henkilökohtaiseen esittelyyn ja harrastusohjelmistoon

Sivuston tyyli on inspiroitu vanhoista tietokoneista, Commodore-tyylisistä käyttöliittymistä ja CRT-näytöistä.

## Ominaisuudet

- retrotyylinen komento-UI
- nopea ja kevyt staattinen HTML-sivu
- ei rakennusvaihetta tai kirjastoja
- mahdollisuus lisätä uusia projekteja muuttamalla `PROGRAMS`-listaa
- F1/F3/F5/F7-pikanäppäimet
- tuki resoluutiolle ja liiketunnistukselle (esim. reduced motion)

## Ohjelmat

- **Colesteroids OG+** – selaimessa pelattava fysiikkapeli.
- **100 päivää** – kyberturvallisuuden johtamisen opetuspeli.
- **HessuTalks** – päästä päähän salattu kysymys- ja palautekanava luennoille ja puheille.

## Rakenne

- `index.html` – koko sovellus ja käyttöliittymä

## Käynnistäminen paikallisesti

Koska projekti on staattinen HTML-sivu, se voidaan avata joko suoraan selaimessa tai palvelimen kautta.

### Vaihtoehto 1: suora avaaminen

Avaa tiedosto selaimessa:

```bash
open index.html
```

### Vaihtoehto 2: paikallinen web-palvelin

```bash
cd /Users/hessu/Projektit/softa
python3 -m http.server 8000
```

Sen jälkeen avaamalla selaimessa:

```text
http://localhost:8000
```

## Muokkaaminen

Päämuutokset tapahtuvat `index.html` tiedostossa. Erityisesti:

- `PROGRAMS`-lista määrittelee näkyvät ohjelmat
- `ABOUT`-lista määrittelee esittelytekstin
- `PAL`-lista määrittelee käyttöliittymän värit
- `help()`-funktio sisältää käytettävissä olevat komennot

## Kehitystila

Projekti on henkilökohtainen portfolio- ja kokeiluympäristö. Uusia pelejä, työkaluja tai projekteja voidaan lisätä myöhemmin samanlaiseen retrokonsolityyliin.

## Lisenssi

Tämä projekti ei sisällä erillistä lisenssiä. Käytä sitä henkilökohtaisiin, kokeellisiin tai portfoliotarkoituksiin.
