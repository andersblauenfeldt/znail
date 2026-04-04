# Znail — Forretningsanalyse og konceptovervejelser

_Udarbejdet april 2026 til intern brug_

---

## 1. Historik og DNA

Znail blev skabt i 1998 af Anders Blauenfeldt og Mikkel Stegmann som universitets-projekt på DTU. Konceptet opstod fra en konkret frustration: de kunne ikke tilgå egne bookmarks og filer fra andre computere end deres egne.

**Originalkonceptet bestod af fire dele:**
- **znail-space** — personlig online diskette (5MB)
- **znail-it** — allestedsnærværende huskeseddel (tekst/noter)
- **znail-marks** — online bookmarks på tværs af maskiner og browsere
- **znail-friends** — kontaktbog (emails, telefonnumre)

Slogans: *"for easier living in a virtual world"* og snegle-metaforen (at bære sit hus på ryggen) var stærke og mindeværdige.

**Milepæle:**
- Okt 1998: znail.dk åbner. Tusindvis af brugere inden for måneder.
- 1999: Solgt til TV2 → relanceret som znail.tv2.dk (navneskifte til "Ping")
- 2001: Anders og Christian Schmidt launcher znail.com internationalt fra bunden
- 2002: TV2 lukker znail.tv2.dk. Donation-model introduceret på znail.com
- Toppen: 898 samtidige brugere online (registreret på forsiden)

**Pressecitater fra den tid:**
> *"et lærestykke i pædagogisk forklaring"* — Alt om Data
> *"sjovt lavet og ganske anvendelig"* — PC World
> *"ny og anderledes måde at bruge Internettet på"* — Politiken
> *"slut med gammeldaws lommebog og blyant"* — Webworld

Znail var i Danmark en pionertjeneste — lanceret **ni år før Dropbox** (2007) og **ti år før Evernote** (2008).

---

## 2. Konkurrentlandskab i 2026

### Fil-opbevaring og sync
| Tjeneste | Gratis | Pris | Styrke | Svaghed |
|---|---|---|---|---|
| Google Drive | 15 GB | fra 100 DKK/md | Integration, ubiquitous | Google scanner indhold, privacy |
| Dropbox | 2 GB | fra 120 DKK/md | Poleret, udbredt | Dyrt, tungt |
| iCloud | 5 GB | fra 11 DKK/md | Gnidningsfrit på Apple | Apple-lock-in |
| OneDrive | 5 GB | inkl. i Microsoft 365 | Godt for Windows-brugere | Microsoft-afhængighed |
| Proton Drive | 1 GB | fra 40 DKK/md | End-to-end krypteret, privacy | Relativt lille brugerbase |

### Midlertidig fildeling (WeTransfer-lignende)
- **SwissTransfer** — gratis, privat, op til 50GB, ingen login
- **Smash** — ingen filstørrelsesbegrænsning, gratis op til 2GB
- **Hostize** — upload og få et link med det samme, ingen login

### Bookmarks / "gem til senere"
- **Raindrop.io** — moderne bookmark-manager, gratis tier, flot UI
- **Pocket** (Mozilla) — læs-det-senere, integreret i Firefox
- **Pinboard** — minimalistisk, betalt ($22 engangs), cult-following

### Noter / huskesedler
- Apple Notes, Google Keep, Notion, Obsidian — alle veletablerede

**Konklusion:** Markedet er dybt og domineret af tech-giganter. Men der er stadig huller — særligt i **simplicitet**, **privacy** og **fildeling uden konto**.

---

## 3. Forretningsmuligheder

### Mulighed A: Nostalgi-relaunch — "Znail Classic"
**Koncept:** Bring det originale znail tilbage, næsten 1:1, men moderniseret teknisk.
- Fil-opbevaring, noter, bookmarks, kontakter i ét simpelt interface
- Målgruppe: Danskere der husker znail + tech-interesserede 30-50 årige
- Revenue: Freemium (gratis 1GB, betalt for mere)

**Fordele:**
- Stærk nostalgisk fortælling — "pioneren er tilbage"
- Brand eksisterer allerede, domæner ejet
- Lav markedsføringsindsats i Danmark via nostalgi-vinkel og presse

**Ulemper:**
- Markedet er fyldt — svært at differentiere på funktion alene
- Nostalgi bærer ikke langt uden et klart why-now
- Dansk brand er begrænset internationalt

---

### Mulighed B: Privacy-first fildeling — "Znail Share"
**Koncept:** Upload en fil, få et link, del det. Ingen konto. Ingen tracking. Ingen AI der scanner dine filer. Sletter automatisk efter X dage.

Positionering: *"WeTransfer without the creepy privacy policy"*

WeTransfer opdaterede i 2023 deres privatlivspolitik til at tillade brug af brugerfiler til kommercielle formål og AI-træning. Det skabte massiv modreaktion og folk leder aktivt efter alternativer.

**Fordele:**
- Klar og enkel value proposition
- Timing er god (WeTransfer-backlash)
- Ingen login = lav friktion = viral potentiale
- Kan skalere simpelt

**Ulemper:**
- Konkurrence fra SwissTransfer, Smash m.fl.
- Svært at monetisere uden login (hvem sender fakturaen til?)
- Znail-brandet er ikke naturligt associeret med "deling"

---

### Mulighed C: Den personlige cloud-skuffe — "Znail Personal"
**Koncept:** En simpel, privat online skuffe til dig selv. Log ind, upload filer, gem noter, tilgå fra alle enheder. Ingen bloat, ingen AI, ingen annoncering. Betalt fra dag ét.

Positionering: *"Din digitale rygsæk — som i 1998, bare bedre"*

**Fordele:**
- Direkte arv af det originale znail-DNA
- Privacy som differentiator (ingen scanning, ingen AI)
- Simpel at bygge og drifte
- Klar betalingsmodel (abonnement)

**Ulemper:**
- Svært at konkurrere med gratis Google Drive på pris
- Kræver folk aktivt vælger privacy over bekvemmelighed

---

### Mulighed D: Znail for teams / small business
**Koncept:** Simpel fildeling og noter til små teams — uden enterprise-kompleksitet.
- Delt filmappe, delte noter, simpel adgangsstyring
- Målgruppe: Freelancere, små firmaer, kreative teams

**Fordele:**
- B2B har bedre betalingsvilje end forbrugere
- Markedet for "simple tools" er stort (Basecamp har vist det)

**Ulemper:**
- Kræver mere udvikling end B2C
- Znail-brandet er ikke naturligt B2B

---

## 4. Omkostningsovervejelser

### Infrastruktur (estimater)
| Scenarie | Brugere | Lager | Server | Månedlig infra-pris |
|---|---|---|---|---|
| Hobby/test | ~100 | 10 GB | VPS 4GB (Hetzner) | ~30 DKK |
| Lille launch | ~1.000 | 100 GB | VPS 8GB + backup | ~150 DKK |
| Voksende | ~10.000 | 1 TB | Dedikeret/object storage | ~500-1.500 DKK |
| Seriøs | ~100.000 | 10 TB | Cloud object storage (S3-lignende) | ~5.000+ DKK |

**Vi har allerede:** VPS med 90GB ledig disk — nok til en første launch.

### Udviklingsomkostninger
- MVP (fil-upload, login, download): 1-2 ugers arbejde
- Betalingssystem (Stripe): +2-3 dage
- Mobil-optimering: +1 uge
- Kryptering: +1-2 uger

### Revenue-modeller
| Model | Fordel | Ulempe |
|---|---|---|
| Freemium (gratis 1GB, betalt for mere) | Lav friktionsindgang | Mange gratis-brugere koster penge |
| Kun betalt (fx 29 DKK/md) | Simpelt, profitabelt fra start | Høj friktion, ingen viral vækst |
| Engangsdonation (som originale znail) | Autentisk, lavt pres | Uforudsigelig indkomst |
| Pay-what-you-want | Nostalgisk, god PR | Svært at budgettere |

---

## 5. Brand og nostalgi-mulighed

### Hvad znail faktisk har
- Et genuint pionerbrand i Danmark — omtalt i Politiken, PC World, Alt om Data, Folkeskolen
- En autentisk founding story (DTU-projekt, 1998, TV2-salg)
- Domænerne znail.dk og znail.com
- Snegle-metaforen er stadig stærk og original

### Hvad nostalgi kan og ikke kan
**Kan:**
- Give pressedækning gratis ("pioneren vender tilbage efter 25 år")
- Aktivere dansk tech-community (LinkedIn, communities)
- Skabe en autentisk fortælling i en verden fuld af startup-hype

**Kan ikke:**
- Bære et produkt der ikke løser et reelt problem i 2026
- Erstatte en klar value proposition
- Skaffe internationale brugere (znail kendes primært i DK)

### PR-vinkel der virker
> *"I 1998 opfandt to DTU-studerende Dropbox og Evernote — men gav dem det forkerte navn. Nu er znail tilbage."*

Dette er en legitim og stærk vinkel. Pressen elsker den slags historier.

---

## 6. Produkt/markeds-fit overvejelser

| Mulighed | Problem-solution fit | Markedsstørrelse | Konkurrence | Byg-kompleksitet | Samlet vurdering |
|---|---|---|---|---|---|
| A: Nostalgi-relaunch | Middel | Lille (DK) | Høj | Middel | ⭐⭐ |
| B: Privacy fildeling | Høj | Stor | Middel | Lav | ⭐⭐⭐⭐ |
| C: Personlig cloud-skuffe | Høj | Middel | Middel | Lav-middel | ⭐⭐⭐⭐ |
| D: Teams | Middel | Middel | Høj | Høj | ⭐⭐ |

---

## 7. Anbefaling til brainstorm

Min vurdering er at **B og C kombineret** er den stærkeste mulighed:

**"Znail — din personlige, private online skuffe"**

- Upload filer, gem noter, del med et link (sletter efter X dage)
- Ingen AI, ingen annoncering, ingen scanning
- Betalt abonnement — eller gratis med begrænsninger
- Znail-brandet bruges aktivt: *"Vi opfandt det i 1998. Nu har vi lavet det ordentligt."*

Det er simpelt at bygge, der er en klar differentiator (privacy), og det har en autentisk story bag sig.

---

## 8. Database og eksisterende brugere

**Adgang:** FTP til 217.116.232.251, user: znail, pass: Znail4Ever2026

**Kodebase:** Original PHP-kode fra 2007-2008 ligger stadig på serveren under `www/znail.com/`

**Database credentials (fra znail.inc.php):**
- Host: localhost (på Gigahost)
- User: znail
- Password: ayttm.rdn
- DB: znail

**Tabeloversigt:**
| Tabel | Rækker | Indhold |
|---|---|---|
| T_users | 15.082 | Brugere (ingen email-kolonne) |
| T_extendeduserinfo | 13.145 | Demografisk data |
| T_user_settings | 15.083 | Email, nyhedsbrev-samtykke |
| T_znailmarks | 547.027 | Gemte bookmarks |
| T_znaildisk_log | 790.853 | Filaktivitet |
| T_login_log | 2.246.367 | Login-historik |
| T_znailnotes | 936 | Gemte noter |
| T_znailfriends | 236 | Kontaktbog |
| T_active_users | 912 | Aktive lige nu |

**Brugerstatus:**
- Aktive brugere (seneste 2 år): **58**
- Aktive brugere (seneste 5 år): **97**
- Brugere med email: **6.433**
- Tilmeldt nyhedsbrev (GDPR-ok): **987**

**Konklusion:** Znail kører stadig og bruges aktivt. 987 emails klar til relancerings-mail når vi er klar.

---

## 9. Relaunch-strategi

### Auth — BESLUTTET: Clerk
Brug **Clerk** til brugeradministration — login, signup, 2FA, password reset, social login.
- **Gratis op til 50.000 MAU** (Auth0 stopper ved 25.000)
- Betalt: $20/md + $0.02 per ekstra bruger over 50k
- GDPR-compliant
- clerk.com

**Opsætning (engangs):**
1. Opret Clerk-konto og app
2. Byg **custom login UI** i Znails eget design — ingen "Powered by Clerk" synlig
3. Konfigurér **custom email domain**: `noreply@znail.com`
   - Tilføj znail.com som afsender i Clerk dashboard
   - Sæt SPF + DKIM DNS-records hos domæne-udbyder
4. Aktivér 2FA (valgfrit for brugeren)
5. Konfigurér password reset-flow med Znail-branding

**Resultat:** Brugeren ser aldrig Clerk — alt ser ud som Znail.

Gamle znail-passwords migreres **ikke** — brugere aktiverer ny konto via email-link.

### Email — BESLUTTET: Brevo
- **Brevo** (brevo.com) til relaunch-mail og nyhedsbreve
- Gratis: 300 emails/dag, ubegrænsede kontakter
- Relaunch-mail til 6.433 brugere: ~22 dage à 300/dag
- Fordel: langsom udsendelse reducerer spam-risiko
- GDPR-compliant, EU-baseret
- Alternativt **Resend** til system-emails fra koden

### Relaunch-mail
- **6.433 emails** i `T_user_settings` — alle med eksisterende konto-relation
- GDPR tillader systemmail med **legitim interesse** (ikke markedsføring)
- Mail-indhold: "Znail er relanceret — dine filer og bookmarks er stadig der. Aktivér din konto her."
- Forventet response: 10-20% = 640-1.200 reaktiverede brugere fra dag ét
- **987 nyhedsbrev-brugere** kan desuden modtage løbende opdateringer

### Migrations-plan
1. Eksportér brugere + emails fra gammel database
2. Importer til Clerk (username + email)
3. Flyt 10.550 filer fra Gigahost til VPS
4. Migrér bookmarks, noter og kontakter til ny database
5. Send relaunch-mail til 6.433 brugere
6. Aktiver ny znail.com

---

## 10. Spørgsmål til afklaring

- Har du lyst til at bygge et seriøst produkt med betalende brugere, eller er det mere et hobby-projekt?
- Er privacy-vinklen vigtig for dig, eller er det mere funktionen der tæller?
- Ønsker du at bygge videre på den originale multi-feature tanke (filer + noter + bookmarks), eller fokusere på ét?
- Har du kontakt til Mikkel Stegmann eller Christian Schmidt som mulige samarbejdspartnere?
