# MESTA Compliance System V2

En moderne, brukervennlig løsning for å administrere underentreprenører, ansatte og dokumentasjon i anleggsprosjekter.

## 🚀 Live Demo

**Åpne og test systemet her:** [DIN GITHUB PAGES URL]

_(Etter GitHub Pages er aktivert, oppdater denne linken)_

## 📋 Hovedfunksjoner

### ✅ Bedriftsadministrasjon
- **Søk i Brønnøysundregistrene** (ekte API)
- **Manuell registrering** med smart validering
- **Kontraktsbasert filtrering** (FV12, E18, etc.)
- **Compliance-sjekker** per bedrift
- **Dokumentkrav** - velg 8 forskjellige dokumenttyper

### ✅ Compliance & Dokumentasjon
- **Påkrevd dokumentasjon** - se hva som mangler (NY!)
- **Status-tracking** (OK, Venter, Utløpt)
- **Visuell feedback** med farger (grønn/gul/rød)
- **Advarsler** for manglende dokumenter
- **8 dokumenttyper**: Skatteattest, MVA, HMS, Forsikring, Ansatteliste, Kvalitet, Miljø, Godkjenning

### ✅ Ansattadministrasjon
- **Registrering** med SMS-varsel til ansatte
- **Dokumentstatus** per ansatt
- **Klikk for detaljer** - se full info i modal (NY!)
- **Kontaktinformasjon** (e-post, telefon)
- **Utløpsdatoer** med automatisk varsling

### ✅ Excel-rapportering
- **Enkeltbedrift**: Detaljert rapport per UE
- **Oversikt**: Samlet rapport med filtrering
- **7 seksjoner**: Sammendrag, Bedrifter, Compliance, Ansatte, Advarsler, Kritiske
- **Respekterer filtreringer** (per kontrakt)
- **UTF-8 BOM** - norske tegn fungerer i Excel

### ✅ API-integrasjoner
- **Brønnøysundregistrene** (aktiv)
- **StartBANK** (demo)
- **Landax HMS** (demo)
- **HMSReg** (demo)
- Test, synkroniser og aktiver/deaktiver

### ✅ Onboarding & Brukeropplevelse
- **3-slides introduksjon** for nye brukere
- **Checkout-mekanisme** (vis maks 2 ganger)
- **"Se introduksjon igjen"** i innstillinger
- **Keyboard shortcuts** (←→, ESC)
- **Responsive design** (PC, tablet, mobil)

### ✅ AI Chat Assistant (mobil)
- **Intelligent chatbot** for ansatte
- **4 quick actions**
- **Demo-funksjon** for dokumentopplasting
- **Gamification** med progress bar og confetti

### ✅ Rollebasert tilgang (NY!)
- **Administrator**: Full tilgang, kan slette UE
- **Prosjektleder**: Kan ikke slette UE (sikkerhet)
- **Underentreprenør**: Ser egen bedrift + compliance

---

## 🎯 Roller & Tilgang

### 👨‍💼 Administrator
- ✅ Full tilgang til alle funksjoner
- ✅ API-administrasjon
- ✅ Alle kontrakter
- ✅ **Slette UE** (kun Admin!)
- ✅ Eksportere rapporter

### 📊 Prosjektleder
- ✅ Administrere bedrifter
- ✅ Registrere ansatte
- ✅ Eksportere rapporter
- ❌ Kan IKKE slette UE (sikkerhet)
- ❌ Kan IKKE endre API-innstillinger

### 🏢 Underentreprenør
- ✅ Se egen bedrifts status
- ✅ **Se påkrevd dokumentasjon** (NY!)
- ✅ Oversikt over ansatte
- ✅ **Klikk på ansatte for detaljer** (NY!)
- ✅ Dokumentstatus (hva mangler)
- ❌ Kan ikke endre data

---

## 🧪 Innlogging (Demo)

Systemet har tre forhåndsvalgte roller:

```
🔐 Login-skjerm:
┌─────────────────────────────┐
│ [👨‍💼 Administrator]          │ ← Klikk her
│ [📊 Prosjektleder]           │ ← Eller her
│ [🏢 Underentreprenør]        │ ← Eller her
└─────────────────────────────┘
```

**Ingen passord nødvendig - bare klikk!**

---

## 📱 Mobil Upload

For ansatte som skal laste opp dokumenter:
- **Fil**: `employee-upload-mobile.html`
- **Gamifisert** opplevelse
- **Progress bar** og confetti-animasjoner
- **AI-assistent** for hjelp

---

## 🗂️ Filstruktur

```
mesta-compliance/
├── index.html                          # ⭐ Hovedapplikasjon
├── employee-upload-mobile.html         # 📱 Mobil opplasting
├── README.md                           # 📖 Dette dokumentet
├── GITHUB_SETUP_GUIDE.md              # 🚀 Setup-guide
├── FINAL_IMPLEMENTATION_SUMMARY.md     # 📋 Komplett oversikt
├── DOCUMENT_REQUIREMENTS_GUIDE.md      # 📄 Dokumentkrav-guide
├── EXCEL_EXPORT_GUIDE.md              # 📊 Excel-guide
├── NEW_FEATURES_SPECIFICATION.md       # 🆕 Nye funksjoner
├── ROLE_BASED_DELETE_RESTRICTION.md    # 🔒 Tilgangskontroll
└── IAM_CIAM_INTEGRATION_PLAN.md       # 🔮 Fremtidig IAM
```

---

## 🎨 Design

- **Farger**: MESTA-palett (Oransje #FF6B35, Blå #004B87, Grønn #00A651)
- **Font**: Poppins (Google Fonts)
- **Animasjoner**: Smooth, moderne transitions
- **Responsivt**: Fungerer på desktop, tablet og mobil
- **Tilgjengelighet**: Keyboard shortcuts, tydelige kontraster

---

## 🔧 Teknologi

- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **No dependencies**: Ingen eksterne libraries
- **API**: Brønnøysundregistrene (offentlig API)
- **Storage**: LocalStorage for onboarding og preferanser
- **Fallback**: Mock-data når API ikke er tilgjengelig

---

## 📊 Data

Systemet bruker mock-data for demonstrasjon:
- **3 forhåndsregistrerte bedrifter** med ansatte
- **9 bedrifter i søkedatabase** (inkl. Ps Anlegg AS)
- **All data forsvinner ved refresh** (trygt å teste)
- **Ingen database påkrevd** (alt i minne)

---

## 🧪 Testing - Kom i gang

### Test 1: Legg til bedrift via søk
```
1. Logg inn som Admin
2. Klikk "➕ Legg til bedrift"
3. Søk på "Ps Anlegg" eller "912561798"
4. Velg bedrift fra resultatliste
5. Skriv inn kontrakt-ID (f.eks. "TEST-2025")
6. Velg dokumentkrav (3 forhåndsvalgt)
7. Klikk "✓ Bekreft og legg til"
8. Success! Bedrift er lagt til
```

### Test 2: Se compliance som UE (NY!)
```
1. Logg inn som "Underentreprenør"
2. Se ny seksjon øverst: "📋 Påkrevd dokumentasjon"
3. Se hvilke dokumenter som mangler (gul)
4. Se hvilke dokumenter som er OK (grønn)
5. Les advarsel hvis noe mangler
```

### Test 3: Klikk på ansatt for detaljer (NY!)
```
1. Logg inn (Admin eller UE)
2. Åpne en bedrift / se ansatte
3. Klikk på en ansatt (se "→" på høyre side)
4. Modal viser: Navn, stilling, e-post, telefon, alle dokumenter
5. Lukk modal
```

### Test 4: Slett UE (kun Admin!)
```
1. Logg inn som Administrator
2. Åpne en bedrift
3. Scroll ned - se rød "🗑️ Slett bedrift" knapp
4. Klikk → Dobbel bekreftelse
5. Bedrift slettes

Prøv som Prosjektleder:
1. Logg inn som Prosjektleder
2. Åpne en bedrift
3. Slett-knappen er BORTE! ✓
```

### Test 5: Excel-export med filtrering
```
1. Velg kontrakt i dropdown (f.eks. "FV12-2025-MESTA")
2. Klikk "📊 Eksporter oversikt til Excel"
3. CSV lastes ned med kun filtrerte bedrifter
4. Åpne i Excel - se 7 seksjoner
```

---

## 🎓 Dokumentasjon

Fullstendig dokumentasjon finnes i `/docs`:
- **FINAL_IMPLEMENTATION_SUMMARY.md** - Komplett oversikt
- **DOCUMENT_REQUIREMENTS_GUIDE.md** - Guide til dokumentkrav
- **EXCEL_EXPORT_GUIDE.md** - Excel-rapportering
- **NEW_FEATURES_SPECIFICATION.md** - Nye funksjoner
- **ROLE_BASED_DELETE_RESTRICTION.md** - Tilgangskontroll
- **IAM_CIAM_INTEGRATION_PLAN.md** - Fremtidig IAM

---

## 🆕 Siste oppdateringer (Februar 2025)

### ✅ Versjon 2.3 - Compliance & Tilgang
- **Compliance-visning for UE**: Se påkrevd dokumentasjon med status
- **Klikk på ansatt**: Modal med full info og dokumenter
- **Rollebasert sletting**: Kun Admin kan slette UE
- **Fargekodet status**: Grønn (OK), Gul (Mangler), Rød (Utløpt)
- **Advarselbokser**: Tydelig feedback på hva som mangler

### ✅ Versjon 2.2 - Dokumentkrav
- **8 dokumenttyper**: Velg ved opprettelse av UE
- **Fleksibelt valg**: Fra 1 til 8 dokumenter per bedrift
- **Excel-export**: Inkluderer valgte dokumentkrav

### ✅ Versjon 2.1 - Kontraktsfiltrering
- **Dropdown-filter**: Filtrer per kontrakt
- **Oversikts-export**: Respekterer valgt kontrakt
- **7 seksjoner**: Omfattende rapportering

### ✅ Versjon 2.0 - Komplett system
- Onboarding, API-integrasjoner, Manuell registrering
- AI Chat Assistant, Excel-export
- Responsive design

---

## 🔮 Fremtidige forbedringer

### V2.4 (Neste sprint)
- [ ] **Sub-UE**: Underentreprenører til underentreprenører
- [ ] **Dokumentopplasting**: Direkte i systemet
- [ ] **Edit dokumentkrav**: Endre etter registrering

### V2.5 (Q2 2025)
- [ ] Bulk-operasjoner
- [ ] Historikk og audit trail
- [ ] Advanced analytics
- [ ] Push-notifikasjoner

### V3.0 (Q3 2025)
- [ ] Native mobile apps
- [ ] Altinn-integrasjon
- [ ] Biometric authentication
- [ ] AI-validering av dokumenter
- [ ] IAM/CIAM (Auth0/Azure AD)

---

## 📞 Support

For spørsmål eller problemer:
- Åpne et GitHub Issue
- Kontakt: [DIN E-POST]

---

## 📄 Lisens

Dette er en demo-applikasjon laget for MESTA.

---

## 🏆 Credits

**Laget med ❤️ for MESTA**

*Siste oppdatering: 12. Februar 2025*
*Versjon: 2.3*

