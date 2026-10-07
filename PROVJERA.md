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

Vizuelni raspored u stvarnom desktop/mobilnom pregledniku nije testiran u ovom okruženju. Responsive CSS i otvaranje mobilnog menija provjereni su u izvoru/DOM-u. Fotografije su vizuelno pregledane odvojeno od rasporeda stranice.

Ovo je lokalni interaktivni demo: prijava bira ulogu, poslovni podaci i ERP tok su demonstracioni, a promjene se čuvaju u pregledniku. Stvarni OCR, produkciona autentifikacija i ERP povezivanje nisu uključeni.
