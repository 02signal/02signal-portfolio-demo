# Nädal 4 — AI Turunduskalender

## Artefakt: UrbanStyle.ltd Automatiseeritud Sisuplaan

### Probleem
Anna toodab 5 sisuühikut nädalas. Konkurendid toodavad 20. UrbanStyle jääb maha.

### Lahendus
n8n workflow, mis genereerib AI abil sisu draft'id turunduskalendri põhjal:

```
Google Sheets (turunduskalender)
    ↓
n8n Schedule Trigger (iga esmaspäev)
    ↓
AI Node (genereerib 5 draft-postitust nädala teemade põhjal)
    ↓
Telegram (saadab draft'id Anna'le kinnitamiseks)
```

### Näidis — Nädala draft'id

| # | Teema | Segment | Kanal | AI Draft |
|---|-------|---------|-------|----------|
| 1 | Uus eco-kollektsioon | Emma | Instagram | "Kas sa tead, et meie uus linane sari on 100%..." |
| 2 | Suuruste juhend | Triin | TikTok | "POV: Sa ei tea, kas S või M..." |
| 3 | Meeste basics | Peeter | Email | "5 ajatut klassikut, mida iga mees vajab" |
| 4 | Flash sale teade | Henri | Telegram | "48h — valitud tooted -30%!" |
| 5 | Kinkeidee | Kati | Instagram | "Ei tea, mida kinkida? Meie AI aitab!" |

### Tulemused
- Sisu kogus: 5 → **15 ühikut nädalas** (Anna toimetab, mitte ei kirjuta nullist)
- Anna aeg: 8h → **3h nädalas**
- Sisu on **segmendipõhine** — iga postitus räägib konkreetse kliendiga

### Micro-win
*"AI genereeris 5 draft'i 2 minutiga. Mul kulus varem 1 tund ühele postitusele."*
