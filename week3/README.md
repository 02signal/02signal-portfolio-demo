# Nädal 3 — Töötav FAQ Bot

## Artefakt: UrbanStyle KKK Telegram Bot

### Mis ma ehitasin
Telegram bot, mis vastab UrbanStyle'i klientide küsimustele automaatselt, kasutades 30 KKK teadmusbaasi ja AI-d.

### Workflow (n8n)
```
Form Trigger (klient täidab vormi)
    ↓
AI Node (otsib vastuse 30 KKK hulgast, genereerib sõbraliku vastuse)
    ↓
Telegram Bot (saadab vastuse kliendile + teavitab meeskonda)
```

### Näidis-vestlus

**Klient:** "Mis on teie tagastuspoliitika?"

**Bot:** "Tere! UrbanStyle'i tagastuspoliitika on lihtne:
- 30 päeva tagastusõigus alates ostukuupäevast
- Toode peab olema kasutamata ja originaalsiltidega
- Tagastus Omniva pakiautomaadist on TASUTA
- Raha tagastatakse 5-7 tööpäeva jooksul

Kas sul on veel küsimusi? 😊"

**Klient:** "Kas Narva pood on pühapäeval avatud?"

**Bot:** "Narva Fama keskuse kauplus on avatud:
- E-R: 10:00-20:00
- L: 10:00-18:00
- P: Suletud

Lähim avatud pühapäeval: Tartu Tasku (10:00-18:00) või e-pood urbanstyle.ee (24/7). 🛍️"

### Tulemused
- Vastamise aeg: 4-6h → **<5 sekundit**
- Toomas'e aja kokkuhoid: **5.4h nädalas**
- 30 KKK katab **~80% klientide küsimustest**

### Toomas'e tsitaat
*"See bot vastab paremini kui meie IT helpdesk. Ja ma ütlen seda kui inimene, kes kolm nädalat tagasi ütles, et AI on hype."*

### Micro-win
*"Ma täitsin vormi ja 3 sekundit hiljem oli Telegramis vastus. See töötab. PÄRISELT."*
