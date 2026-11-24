# Potrebne fotografije

Stranica trenutačno prikazuje rezervirana mjesta (placeholdere). Kad fotografija stigne, spremite je u
`src/assets/photos/` pod točnim nazivom iz tablice (npr. `src/assets/photos/portret-direktora.jpg`) i ponovno
objavite stranicu. Placeholder se sam zamijeni, a stranica sama napravi AVIF i WebP inačice u više širina.

Dopušteni formati izvornika: `.jpg`, `.jpeg`, `.png`, `.webp`, `.avif`. Fotografije moraju biti klijentove
(vlastite ili s pisanim dopuštenjem autora). Ne koristiti fotografije s demo stranice ni iz banke slika.

| Naziv datoteke | Omjer | Najmanja rezolucija | Kadar | Gdje se prikazuje |
| --- | --- | --- | --- | --- |
| `portret-direktora.jpg` | 4:5 (uspravno) | 1200 × 1500 px | Dejan Softić, do pojasa ili do prsa, na gradilištu ili ispred kamenog zida; prirodno svjetlo, pogled u kameru | Početna, O nama |
| `novogradnja-vanjski.jpg` | 3:2 | 2400 × 1600 px | Dovršena ili gotovo dovršena novogradnja, cijela kuća s okolišem, bez automobila i ljudi u prvom planu | Novogradnja, Reference |
| `gradiliste-dizalica.jpg` | 3:2 | 2400 × 1600 px | Gradilište u fazi grubih radova: armatura, oplata ili zidanje, po mogućnosti s dizalicom | Grubi radovi, Reference |
| `adaptacija-prije.jpg` | 4:3 | 2000 × 1500 px | Stara kamena kuća prije radova; zapamtiti mjesto i visinu snimanja | Adaptacija kamenih kuća, Reference |
| `adaptacija-poslije.jpg` | 4:3 | 2000 × 1500 px | Ista kuća nakon radova, iz istog kuta i s iste visine kao "prije" | Adaptacija kamenih kuća, Reference |
| `fuga-detalj.jpg` | 1:1 | 1600 × 1600 px | Krupni plan očišćenog i ponovno fugiranog kamenog zida, koso svjetlo da se vidi reljef | Reference |
| `zavrsni-kupaonica.jpg` | 3:2 | 2400 × 1600 px | Dovršena kupaonica ili drugi završni radovi (keramika, žbuka, pod), uredno i bez alata | Završni radovi, Reference |
| `potporni-zid.jpg` | 3:2 | 2400 × 1600 px | Potporni zid obložen lokalnim kamenom, po mogućnosti uz stari suhozid, stepenice ili terasu | Potporni zidovi, terase i bazeni, Reference |
| `tim-na-terenu.jpg` | 3:2 | 2400 × 1600 px | Radnici na gradilištu u radu, sa zaštitnom opremom; potrebna je privola osoba na fotografiji | Reference |

## Napomene

- Vodoravne fotografije snimati s ravnim horizontom, bez širokokutnog izobličenja.
- Fotografije "prije" i "poslije" vrijede samo ako su iz istog kuta.
- Za osobe koje se mogu prepoznati (portret, tim) potrebna je njihova privola za objavu.
- Dok postoji barem jedan placeholder, u podnožju stoji napomena "Fotografije na stranici su ilustracije." i stranica
  Reference se ne indeksira. Kad stignu sve fotografije, u `src/i18n/routes.ts` maknite `references` iz popisa `NOINDEX`.
- Popis mjesta za fotografije je u `src/lib/photos.ts`. Novo mjesto dodaje se ondje i u prijevode (`photos.slots`).
