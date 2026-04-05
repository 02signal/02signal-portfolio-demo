# Demo Juhend — Kuidas Seda Repo't Sessioonil Näidata

**Kasutus:** N1 S1, GitHub demo osa (~15 min)
**Eesmärk:** Tekitada "wow" ja "ma tahan ka seda!" reaktsioon

---

## Demo 1: GitHub kui Portfoolio (3 min)

1. Ava brauseris see repo
2. Näita README.md — teekonna kaart (7 nädalat, iga nädal artefakt)
3. Kliki `week1/` → näita kliendisegmentide raport
4. Kliki `week3/` → näita FAQ boti kirjeldus + näidis-vestlus
5. Ütle: *"See on portfoolio, mis teil 7 nädala pärast valmis saab. Iga nädal lisate ühe sellise artefakti."*

## Demo 2: GitHub + Claude Projekt = AI Teadmusbaas (7 min) ← WOW

**See on kõige olulisem demo!**

### Ettevalmistus (enne sessiooni):
1. Loo Claude'is uus Projekt: "UrbanStyle AI Teadmusbaas"
2. Lisa projektifailideks `knowledge-base/` kausta **kõik 8 faili**:
   - urbanstyle-overview.md — ettevõtte profiil
   - customer-segments.md — kliendisegmendid
   - processes-automation.md — protsessid
   - faq-knowledge.md — klienditeeninduse KKK
   - pricing-and-discounts.md — hinnareeglid ja allahindlused
   - brand-voice-and-tone.md — brändi hääl ja kirjutamisstiil
   - new-employee-onboarding.md — uue töötaja juhend
   - seasonal-calendar.md — hooajakalender ja kampaaniad

### Sessiooni ajal:

**Samm 1: Ilma teadmusbaasita (2 min)**

Ava TAVALINE Claude vestlus (mitte Projekt) ja küsi:
```
Mis on UrbanStyle'i tagastuspoliitika?
```
→ AI annab üldise vastuse (ei tea konkreetset poliitikat)

**Samm 2: Teadmusbaasiga (3 min)**

Ava Claude PROJEKT (kus failid on lisatud) ja küsi SAMA küsimus:
```
Mis on UrbanStyle'i tagastuspoliitika?
```
→ AI vastab TÄPSELT: "30 päeva, Omniva tasuta, 5-7 tööpäeva..."

**Reaktsioon:** Osalejad näevad vahet. Ütle: *"See on SAMA AI. Erinevus on teadmusbaas — teie GitHub repo."*

**Samm 3: Ärilised küsimused (2 min)**

Küsi Claude Projektis veel:
```
Millist kliendisegmenti peaks UrbanStyle esmalt AI-ga teenindama ja miks?
```
→ AI vastab detailselt: Eco-teadlik Emma, 35%, kõrgeim lojaalsus, 3 pain point'i...

```
Koosta Narva poe turundusplaan meeste segmendile
```
→ AI kasutab kõiki faile: poe andmed + segmendid + protsessid

```
Uus töötaja alustab Pärnu poes homme. Mida ta peab teadma esimesel päeval?
```
→ AI kombineerib onboarding juhendi + poe eripärad + hooajainfo

```
Kirjuta kliendile vastus, kes küsib allahindlust eco-tootele. Kasuta meie brändi häält.
```
→ AI teab: eco-tooted EI osale flash sale's + vastab "sina"-vormis, sõbralikult

### Punchline:

> *"Teie GitHub portfoolio EI OLE lihtsalt failide hoidmine. See on teie äri AI mälu. Mida rohkem te sinna lisate, seda targemaks teie AI muutub. Ja 7 nädala pärast on teil teadmusbaas, mis teab teie ärist rohkem kui ükski uus töötaja."*

## Demo 3: Tulevik — N3 Bot Teaser (2 min)

Näita `week3/README.md` ja ütle:
*"3 nädala pärast ehitate te päriselt sellise boti. Mitte demo — töötava boti, mis vastab klientidele Telegramis. Ja ta kasutab SEDA SAMA teadmusbaasi, mille te GitHubis loote."*

---

## Oluline

- **ÄRGE näidake kõiki nädalaid** — ainult week1 (kliendid) ja week3 (bot). Ülejäänud on osalejate jaoks "teaser" — nad näevad, et neid ootab midagi ees.
- **Fookus on VÄÄRTUSEL**, mitte GitHubi UI-l. GitHub on tööriist, AGA väärtus on AI teadmusbaas.
- **Osalejad ei pea teadma kõiki tehnilisi detaile** — nad peavad TUNDMA, et see on ägedaim asi, mida nad teha saavad.
