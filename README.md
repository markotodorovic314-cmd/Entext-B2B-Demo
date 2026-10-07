# ENTEXT · B2B Partner Portal

Kompletan interaktivni demo za prezentaciju Entextu. Statički HTML/CSS/JavaScript paket: radi na GitHub Pages bez instalacije, bez build koraka i bez server aplikacije.

## Postavljanje na GitHub Pages

1. Raspakujte ZIP na računaru.
2. U GitHub repozitorij prenesite **cijeli sadržaj raspakovanog paketa**, uključujući fascikle `assets`, `vendor` i `primjeri`.
3. `index.html` mora biti direktno u korijenu repozitorija, uz `app.js`, `data.js` i `styles.css`. Ne prenosite samo ZIP i ne ostavljajte fajlove u dodatnoj fascikli unutar repozitorija.
4. Otvorite **Settings → Pages → Build and deployment → Deploy from a branch**.
5. Izaberite **main** i **/ (root)**, pa **Save**.
6. Otvorite link koji GitHub prikaže nakon objave. Ako vidite prethodnu verziju, osvježite pomoću **Ctrl+F5**.

Sve putanje su relativne. Paket radi i na adresi tipa `https://username.github.io/entext-demo/`. Nije potrebno mijenjati putanje u skriptama. Za brz lokalni pregled otvorite `index.html` u pregledniku; za prezentaciju i dosljedno pamćenje promjena preporučuje se GitHub Pages.

## Demo pristup

Najbrži ulaz: klik na ponuđeni profil na početnom ekranu. U kartici **Administracija** nalazi se Entext admin profil.

| Profil | E-mail | Lozinka |
| --- | --- | --- |
| Izvođač · Adria Build | izvodjac@demo.entext.me | Demo2026! |
| Hotel · Aurora | hotel@demo.entext.me | Demo2026! |
| Trgovac · blokiran kredit | trgovina@demo.entext.me | Demo2026! |
| Administracija | admin@demo.entext.me | Demo2026! |

U administraciji postoje još arhitektonski studio, investitor i instalater. Za njihov prikaz otvorite **Partneri → Pogled kupca**. Nazivi partnera, kontakt podaci i poslovni uslovi su izmišljeni demo podaci.

## Šta možete pokazati na sastanku

1. Uđite kao **Adria Build**. Otvorite katalog, pretragu i detalje proizvoda.
2. Dodajte materijale u korpu. Izaberite skladište, adresu gradilišta i referencu, zatim pošaljite demo narudžbinu.
3. Odjavite se i uđite u **Administraciju**. U narudžbinama otvorite novi zahtjev i promijenite status u **Potvrđena**, zatim **U pripremi** ili **Otpremljena**.
4. Vratite se na kupca. Promijenjen status, istorija i dokument dostupni su u njegovim narudžbinama.
5. U katalogu otvorite keramiku i isprobajte kalkulator m² sa rezervom za rezanje. Iz korpe napravite projektnu ponudu i pokažite admin obradu zahtjeva.

Za kreditnu blokadu uđite kao **Mont Pro trgovina**. Narudžbina se čuva kao blokirana, uz razlog blokade. Administrator može urediti limit, dugovanje i blokadu partnera, pa odobriti narudžbinu.

## Funkcionalnosti

- Kupčev i admin portal, prijava preko demo profila, odjava bez brisanja podataka.
- 44 odabrana stvarna proizvoda iz javnog Entext asortimana (kompletan demo katalog): kupatilo, keramika, podovi, građevinski program, vodovod i namještaj.
- Svih 44 artikla imaju lokalno spakovanu fotografiju; rezervni prikazi služe samo ako fotografija ne može da se učita. Izvori proizvoda i fotografija evidentirani su u `izvori.csv`.
- Katalog u karticama i tabeli; pretraga po šifri, nazivu, brendu i specifikaciji; filteri po kategoriji, brendu, dostupnosti i partner izboru; sortiranje; stranice i favoriti.
- Detalji artikla sa originalnim specifikacijama koje su dostupne na izvoru, jedinicom naručivanja, cijenom, rabatom i stanjem po skladištima.
- Asortiman po partneru. Administrator bira kategorije koje kupac vidi; neoznačene kategorije znače da je dozvoljen cijeli katalog.
- Individualni rabati i demo količinska pravila **10 / 20 / 30%**. Primjenjuje se povoljniji rabat; procenti se ne sabiraju.
- Korpa, promjena količine, čuvanje i učitavanje korpe, obračun osnovice i demo PDV-a, provjera raspoloživosti u izabranom skladištu, minimalne narudžbine i kreditnog limita.
- Dostava na gradilište ili adresu, lično preuzimanje, željeni datum, referenca projekta i napomena.
- Brza narudžbina po demo šifri, originalnoj Entext šifri kada je navedena na izvoru ili nazivu; pojedinačno i unos više redova; provjera nepoznatih šifri i neispravnih količina. Podržani su nazivi sa zarezima unutar CSV navodnika.
- Stvarno čitanje **CSV, TXT, XLSX i XML** fajlova. Primjeri za sva četiri formata nalaze se u `primjeri`.
- Fotografija/PDF uvoz koristi **jasno označen pripremljeni demo primjer** sa nepoznatim artiklom za provjeru. OCR nije implementiran.
- 18 početnih narudžbina sa više statusa; nove narudžbine, admin potvrda, istorija obrade, blokade, ponavljanje i otkazivanje.
- Rezervacija zalihe i kredita. Otkazivanje vraća rezervaciju; isporuka prenosi rezervisani iznos u demo dugovanje.
- PDF potvrde, demo računi/otpremnice, ponuda iz korpe i projektne ponude; cjenik CSV/XLSX/PDF; izvoz narudžbina, zaliha i izvještaja.
- Projektni zahtjevi sa objektom, adresom, fazom radova, rokom i napomenom; admin status ponude; kupčevo prihvatanje i prenos u korpu po aktuelnim uslovima.
- Kalkulator keramike/podova: površina, procenat rezerve, zaokruživanje na cijele kutije i dodavanje izračunate količine.
- Profil kupca, ugovoreni rok plaćanja, kreditni limit, dugovanje, rezervisani iznos i razlog blokade.
- Partner klub, Silver/Gold/Platinum profili, bodovi i evidentiranje demo nagrada.
- Upiti i reklamacije; kupac kreira zahtjev, administrator mijenja status.
- Admin pregled zahtjeva koji traže pažnju, partneri, rabati, limiti, asortiman, zalihe, pravila odobravanja, izvještaji i dnevnik aktivnosti.
- ERP/WMS tok prikazan kao simulacija, sa dugmetom za evidentiranje demo sinhronizacije.
- Prilagođeni rasporedi za telefon i tablet, mobilni meni i dijalozi sa detaljima.

Iz šireg istraživanja 56 artikala, u završni demo odabrana su 44 za koja je pribavljena fotografija. To je izbor asortimana za prezentaciju, a ne kompletna Entext baza. Fotografije identičnih modela namještaja i lampe sa drugih javnih izvora navedene su u `izvori.csv`. Za varijante pakovanja uz naziv artikla prikazana je napomena ako javna fotografija prikazuje drugo pakovanje.

## Granice demonstracije

Ovo je prototip za sastanak, sa lokalnim demo podacima. Poslovne cijene, rabati, količine, skladišta, kreditni limiti, program lojalnosti i kupci nisu stvarni Entext podaci. Šifre `ENT-xxx` su demo šifre. Dostupne originalne Entext šifre sa izvora prikazane su u detaljima i u `izvori.csv`.

Jedinice naručivanja i pokrivenost kutije su demonstracioni parametri. Kalkulator jasno prikazuje demo pokrivenost; stvarno pakovanje i količine moraju se potvrditi prije stvarne nabavke. Izvorne dimenzije, završne obrade i drugi provjereni podaci prikazani su zasebno.

Obračun koristi jedinstvenu **demo stopu PDV-a 21%**. Izvezeni PDF dokumenti nose oznaku **DEMO** i nisu stvarni računi.

Prijava služi izboru demo uloge. Podaci se pamte u `localStorage` ovog preglednika; demo prijava u `sessionStorage`. Različiti uređaji/preglednici ne dijele promjene. Nema stvarne autentifikacije, slanja e-maila, plaćanja, ERP veze niti serverske baze podataka. Izabrani ERP tek treba potvrditi i povezati.

Reset je dostupan samo kroz **Administracija → Postavke → Vrati početne podatke**. **Odjavi se** zadržava unesene narudžbine i ostale promjene.

## Provjera paketa

Funkcionalni tokovi provjereni su kroz DOM simulaciju: kupčev/admin meni, detalji, rabati, narudžbine, rezervacije, kreditna blokada, odobravanje, otkazivanje, uvoz četiri formata, stvarno generisanje PDF-a, XLSX/CSV izvoz, projektna ponuda, kalkulator, upiti, lojalnost i odjava. Nisu zabilježene JavaScript greške u tim provjerama.

Provjereni su detalji svih 44 artikla, originalne šifre za brzu narudžbinu, CSV nazivi u navodnicima, uklanjanje prethodnog pregleda nakon greške uvoza, negativne količine, čuvanje korpe, minimalna narudžbina i mobilni meni. Sve slike su otvorene i provjerene kao datoteke, a zajednički pregled fotografija pregledan je vizuelno. Izvještaj je u `PROVJERA.md`.

Vizuelna provjera rasporeda u stvarnom pregledniku nije bila dostupna u okruženju izrade. Rasporedi za mobilne uređaje definisani su u CSS-u; prije sastanka otvorite objavljeni GitHub Pages link na svom računaru i telefonu.

## Fajlovi

| Fajl / fascikla | Sadržaj |
| --- | --- |
| `POCNI-OVDJE.txt` | Kratko uputstvo za pokretanje i GitHub |
| `index.html` | Početna stranica i relativne putanje |
| `app.js` | Interakcije i demo poslovni tokovi |
| `data.js` | Entext proizvodi, lokalne slike i demo cijene |
| `styles.css` | Izgled i responsive rasporedi |
| `assets` | Fotografije, ilustrativni rezervni prikazi i ikona |
| `vendor` | Lokalne XLSX i PDF biblioteke sa licencama |
| `primjeri` | CSV/TXT/XLSX/XML narudžbine za testiranje |
| `PROVJERA.md` | Rezultat provjere i ograničenja testiranja |
| `izvori.csv` | Izvori javnog asortimana i fotografija |
| `.nojekyll` | GitHub Pages statičko posluživanje |

Fotografije i robne marke pripadaju njihovim vlasnicima. Paket je pripremljen kao poslovni prezentacioni koncept za Entext.
