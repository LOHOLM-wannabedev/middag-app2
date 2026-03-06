# 🍽 Middagsplanlegger

En AI-drevet webapp som genererer personlige ukemenyer og handlelister basert på dine preferanser.

---

## 📱 Om appen

Middagsplanleggeren er en Progressive Web App (PWA) som kan installeres på mobilens hjemskjerm uten App Store. Den bruker Claude AI (Anthropic) til å lage skreddersydde middagsforslag og automatiske handlelister.

**Live app:** [https://loholm-wannabedev.github.io/middag-app2](https://loholm-wannabedev.github.io/middag-app2)

---

## ✨ Funksjoner

- Generer ukemeny for 7 dager basert på personlige kriterier
- Tilpass matpreferanser, diett, tidsbruk, budsjett og vanskelighetsgrad
- Automatisk handleliste sortert etter kategori
- Bytt ut enkeltretter med ett klikk
- Fjern dager du ikke trenger (ferie, take-out osv.)
- Huk av varer i handlelisten mens du handler
- Fungerer som mobilapp (PWA) på både iPhone og Android

---

## 🛠 Teknologi

| Komponent | Teknologi |
|-----------|-----------|
| Frontend | HTML, CSS, JavaScript (én fil) |
| AI | Claude API (Anthropic) – modell: claude-opus-4-6 |
| Hosting | GitHub Pages (gratis) |
| Lagring | localStorage (lokalt i nettleseren) |
| Installasjon | Progressive Web App (PWA) |

### Arkitektur

```
Bruker (nettleser/mobil)
        ↓
GitHub Pages (hosting)
        ↓
index.html (app)
        ↓
Anthropic API (AI)
```

Appen har ingen egen server eller database. All data lagres lokalt i brukerens nettleser.

---

## 🚀 Kom i gang

### Forutsetninger

- En nettleser (Edge, Chrome, Safari)
- En API-nøkkel fra [console.anthropic.com](https://console.anthropic.com)

### Bruk

1. Åpne appen i nettleseren
2. Gå til **🔑 Nøkkel** og lim inn din Anthropic API-nøkkel
3. Gå til **⚙️ Kriterier** og velg dine preferanser
4. Trykk **✨ Generer ukemeny**
5. Bruk **🔄 Bytt** eller **🗑 Fjern** på enkeltdager etter behov
6. Se handlelisten under **🛒 Handleliste**

### Installer som mobilapp

**Android:** Chrome → tre prikker → «Legg til på startskjermen»

**iPhone:** Safari → Del-ikon → «Legg til på Hjem-skjermen»

---

## 🔐 Sikkerhet og API-nøkkel

- API-nøkkelen lagres kun lokalt i nettleseren via `localStorage`
- Nøkkelen lastes aldri opp til GitHub eller noen server
- Hver bruker må ha sin egen API-nøkkel fra Anthropic
- Sett et månedlig spend limit i Anthropic-konsollen for å unngå uventede kostnader

---

## 📁 Prosjektstruktur

```
middag-app/
├── index.html        # Hele appen (HTML, CSS og JavaScript)
├── .gitattributes    # Git-konfigurasjon
└── README.md         # Denne filen
```

---

## 🗺 Fremtidige funksjoner (roadmap)

- [ ] Eksporter handleliste som tekst
- [ ] Lagre favorittmiddager
- [ ] Full oppskrift med fremgangsmåte
- [ ] Se tidligere ukeменyer
- [ ] Familiedeling med synkronisering
- [ ] Backend-server slik at brukere slipper egen API-nøkkel

---

## 📝 Endringslogg

| Dato | Endring |
|------|---------|
| 06.03.2026 | Første versjon – ukemeny og handleliste |
| 06.03.2026 | La til bytt og fjern-knapper per dag |

---

## 👨‍💻 Utvikling

Bygget med vibe coding ved hjelp av Claude AI som kodepartner.

### Lokal utvikling

1. Klon repoet
2. Åpne mappen i VS Code
3. Høyreklikk på `index.html` → **Open with Live Server**
4. Appen kjører på `http://127.0.0.1:5500`

---

*Laget av LOHOLM-WANNABEDEV*
