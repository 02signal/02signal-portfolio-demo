# Nädal 5 — Andmepõhine Aruandlus

## Artefakt: UrbanStyle.ltd Automaatne Müügiaruanne

### Probleem
Marko kulutab 45 minutit iga hommik müügiaruande koostamisele. Andmed on Google Sheets'is, aga koondamine on manuaalne.

### Lahendus
```
Schedule Trigger (iga tööpäev kell 8:00)
    ↓
Google Sheets (loe eilse müügiandmed)
    ↓
AI Node (koosta kokkuvõte + tuvasta anomaaliad)
    ↓
Telegram (saada aruanne juhtkonna gruppi)
    ↓
Google Sheets (salvesta aruanne arhiivi)
```

### Näidis — Automaatne Hommikuaruanne

> 📊 **UrbanStyle Päevaaruanne — 14.05.2026**
>
> **Käive:** 4,230 EUR (+12% vs eelmine E)
> **Tellimused:** 67 (e-pood 43, Tallinn 12, Tartu 8, Pärnu 4)
> **Top toode:** Linane jakk #1089 (8 müüki)
>
> ⚠️ **Anomaalia:** Narva käive -35% vs eelmine nädal. Põhjus: laoseisu probleem kategoorias "naiste kleidid" (3 toodet out-of-stock).
>
> 💡 **AI soovitus:** Täiendage Narva naiste kleitide laoseisu. Prognoos: 2-päevane tarnetsükkel taastab müügitaseme.
>
> 📈 Nädala trend: [graafik]

### Tulemused
- Marko ajakulu: **45min/päev → 0 min**
- Aruanne valmis: **kell 8:01** (varem kell 9:30)
- Anomaaliad tuvastatakse **automaatselt** — ei pea ise otsima
- Andmed salvestatakse arhiivi → ajaloo analüüs võimalik

### Micro-win
*"Aruanne oli postkastis enne, kui ma hommikukohvi sain. Ja see leidis Narva laoprobleemi, mida ma poleks enne kolmapäeva märganud."*
