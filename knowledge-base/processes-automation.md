# UrbanStyle.ltd — Protsesside Automatiseerimisplaan

## TOP 10 automatiseerimiskandidaati

Liis Koppeli 47 manuaalsest protsessist on tuvastatud 10 kõige mõjukamat automatiseerimiskandidaati:

| # | Protsess | Praegune aeg | Auto. potentsiaal | Ajakokkuhoid | Prioriteet |
|---|----------|-------------|-------------------|-------------|-----------|
| 1 | Kliendi KKK vastamine | 6h/nädal | 90% | 5.4h/nädal | **P0** |
| 2 | Igapäevane müügiaruanne | 45min/päev | 95% | 3.5h/nädal | **P0** |
| 3 | Laoseisu kontroll | 2h/nädal | 85% | 1.7h/nädal | P1 |
| 4 | Sotsiaalmeedia sisu | 8h/nädal | 60% | 4.8h/nädal | P1 |
| 5 | Tellimuse staatus-päring | 3h/nädal | 80% | 2.4h/nädal | P1 |
| 6 | Uue töötaja onboarding | 4h/inimene | 50% | 2h/inimene | P2 |
| 7 | Hankija tellimus | 1h/nädal | 70% | 0.7h/nädal | P2 |
| 8 | Klienditagasiside kogumine | 2h/nädal | 75% | 1.5h/nädal | P2 |
| 9 | Kampaania tulemuse analüüs | 3h/kampaania | 65% | 2h/kamp. | P2 |
| 10 | Töögraafiku koostamine | 2h/nädal | 40% | 0.8h/nädal | P3 |

**Kokku potentsiaalne kokkuhoid: ~23h nädalas = 0.6 FTE**

---

## Protsess #1: Kliendi KKK vastamine (P0)

### Praegune olukord
- Toomas vastab 14+ korda päevas samadele küsimustele
- Peamised teemad: tagastuspoliitika (30%), lahtiolekuajad (20%), suurused (15%), saadavus (15%), muud (20%)
- Keskmine vastamise aeg: 2-6 tundi
- Kanalid: email, Instagram DM, Facebook

### Automatiseerimislahendus
**n8n workflow: Form/Telegram → AI (faq_30 põhjal) → Telegram vastus**

Workflow loogika:
1. Klient saadab küsimuse (Telegram bot / veebivorm)
2. AI node analüüsib küsimust ja otsib vastuse 30 KKK hulgast
3. Kui vastus leidub → automaatne vastus kliendile (<5 sekundit)
4. Kui ei leia → edastab Toomasele (manuaalne vastus + uus KKK kirje)

### Mõõdikud
- Vastamise aeg: 2-6h → <5 sekundit (99% parem)
- Toomas'e aja kokkuhoid: 6h/nädal → 0.5h/nädal
- Kliendirahulolu: eeldatav tõus 15-20% (kiire vastus)

---

## Protsess #2: Igapäevane müügiaruanne (P0)

### Praegune olukord
- Marko koostab iga hommik müügiaruande käsitsi
- Aeg: ~45 minutit (andmete kogumine + formateerimine + saatmine)
- Saajad: Kristi (CEO), Anna (turundus), Liis (operatsioonid)

### Automatiseerimislahendus
**n8n workflow: Schedule (iga päev 8:00) → andmed Google Sheets'ist → AI kokkuvõte → Telegram/email**

1. Ajastatud trigger: iga tööpäev kell 8:00
2. Google Sheets node: loe eilse päeva müügiandmed
3. AI node: koosta kokkuvõte (käive, top tooted, anomaaliad)
4. Telegram: saada aruanne juhtkonna gruppi

### Mõõdikud
- Ajakulu: 45min/päev → 0 min (täisautomaatne)
- Aruanne valmis: kell 9:30 → kell 8:01
- Marko saab keskenduda analüüsile, mitte andmete kokkukorjamisele

---

## Protsess #4: Sotsiaalmeedia sisu (P1)

### Praegune olukord
- Anna toodab 5 sisuühikut nädalas, vaja 20
- Sisu loomine: 1.5h/postitus (foto+tekst+hashtag'id)
- Puudub planeerimine — tehakse "tulekahju" korras

### Automatiseerimislahendus
**n8n workflow: Turunduskalender → AI sisu genereerimine → Draft Telegram gruppi → Anna kinnitab → Avaldamine**

1. Turunduskalender Google Sheets'is (kuupäev, teema, segment, kanal)
2. n8n loeb nädala postitused
3. AI genereerib draft'id (tekst + hashtag'id + CTA)
4. Anna saab Telegramis draft'id → kinnitab/muudab
5. Avaldamine vastavalt kalendrile

### Mõõdikud
- Sisu kogus: 5 → 15-20 ühikut nädalas
- Anna aeg: 8h → 3h (AI genereerib, Anna toimetab)
- Kvaliteet: ühtlasem, segmendipõhine sisu

---

## Narva Poe Case Study

### Mis läks valesti?
Narva poe avamine 2025 alguses nõudis 47 manuaalset sammu. Liis Koppel tegeles kõigega ise:
- Laoseisu sisestamine: 3 päeva käsitsi tööd
- Personalivalik ja koolitus: 2 nädalat
- IT seadistamine: 1 nädal (Toomas pidi Narvas kohapeal olema)
- Kohalik turundus: Anna ei jõudnud — kampaania hilines 2 nädalat

**Tulemus:** Narva poe konversioon 2.1% (keskmine 3.4%). Esimese kuu käive 40% alla oodatu.

### Kuidas AI aitaks Riia avamist?
Automatiseerides 47-st protsessist 28 (60%):
- Laoseisu import: automaatne CSV → süsteem (30 min vs 3 päeva)
- Onboarding materjalid: AI-genereeritud, lokaliseeritud (2h vs 2 nädalat)
- Turunduskampaania: AI sisu + automaatne ajakava (1 päev vs 2 nädalat)
- Aruandlus: automaatne alates päevast 1

**Hinnanguline kokkuhoid:** 120h tööaega, 3 nädalat kiirema avamise
