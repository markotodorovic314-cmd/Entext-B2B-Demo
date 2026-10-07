# Provjera ENText B2B demo paketa

Datum: 7. oktobar 2026. Rezultat: **prošlo**.

- 44 jedinstvena proizvoda sa pojedinačnim detaljima i lokalnim fotografijama.
- Svaka fotografija i showroom slika otvorene su i provjerene: nema oštećenih slikovnih datoteka.
- Pregled svih fotografija vizuelno provjeren u odnosu na tip/model artikla. Javne fotografije različitog pakovanja nose napomenu.
- Izvori pokrivaju svih 44 artikla; primjeri CSV/TXT/XLSX/XML spakovani su uz portal.
- Funkcionalni tokovi prošli su kroz DOM simulaciju: kupac/admin, katalog, favoriti, detalji, korpa, rabati i PDV, zalihe, kredit, blokade, odobravanje, otkazivanje, isporuka, ponavljanje, projekti, kalkulator, lojalnost, upiti, dokumenti i odjava.
- Uvoz četiri formata, originalna Entext šifra, citirani CSV nazivi, neispravan XML, negativne količine, sačuvana korpa i minimalna vrijednost narudžbine provjereni su dodatno.
- PDF izlaz provjeren je kao stvaran PDF; XLSX izlaz kao radna sveska. CSV izlaz je provjeren.
- JavaScript sintaksa prolazi; u funkcionalnim testovima nema JavaScript grešaka.
- Sve putanje za pokretanje i slike su relativne, za GitHub Pages repozitorij u podputanji.

Naknadna provjera objavljenog GitHub Pages portala, 7. oktobar 2026:

- Ispravljene su putanje nakon uploada koji je stavio sve fajlove u korijen. Vraćene su fascikle `assets`, `vendor` i `primjeri`, uključujući sve fotografije i biblioteke.
- Sve 44 različite fotografije na četiri stranice kataloga učitavaju se u stvarnom desktop pregledniku (`complete` i `naturalWidth > 0`); nije korišćena nijedna rezervna ilustracija.
- Kružići kategorija imaju jednaku lijevu poziciju i širinu 16 px; tekst svih kategorija počinje u istoj koloni. Filter Kupatilo i slika u detaljima potvrđeni su kroz UI.
- Portal koristi crno-bijeli ENText identitet. Pregledani su prijava sa fotografijom showrooma, pregled kupca i katalog.
- PDF potvrda i XLSX cjenik preuzeti su iz objavljenog portala. Potvrđeni su PDF zaglavlje i struktura Excel radne sveske.
- Ponovljeno je svih 25 grupa funkcionalnih DOM provjera: prolaze bez JavaScript grešaka.
- GitHub Pages objava za commit `b3b49ad9afda269fc569d1eff6a9b1e9df8d8173` završena je uspješno.

Vizuelni raspored na telefonu nije testiran. Responsive CSS i otvaranje mobilnog menija provjereni su u izvoru/DOM-u.

Ovo je lokalni interaktivni demo: prijava bira ulogu, poslovni podaci i ERP tok su demonstracioni, a promjene se čuvaju u pregledniku. Stvarni OCR, produkciona autentifikacija i ERP povezivanje nisu uključeni.
