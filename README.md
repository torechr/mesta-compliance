# MESTA Compliance System V2

En moderne, brukervennlig løsning for å administrere underentreprenører, ansatte og dokumentasjon i anleggsprosjekter.

## 🚀 Live Demo

**Test systemet her:** [KOMMER ETTER DEPLOY]

## 📋 Funksjoner

### ✅ Bedriftsadministrasjon
- Søk i Brønnøysundregistrene (ekte API)
- Manuell registrering med validering
- Kontraktsbasert filtrering
- Compliance-sjekker per bedrift

### ✅ Dokumentkrav
- 8 forskjellige dokumenttyper
- Fleksibel valg ved registrering
- Status-tracking (OK, Venter, Utløpt)
- Visuell feedback med farger

### ✅ Excel-rapportering
- Enkeltbedrift: Detaljert rapport
- Oversikt: Samlet rapport med alle bedrifter
- 7 seksjoner: Sammendrag, Bedrifter, Compliance, Ansatte, Advarsler, Kritiske
- Respekterer filtreringer

### ✅ API-integrasjoner
- Brønnøysundregistrene
- StartBANK
- Landax HMS
- HMSReg
- Test, synkroniser og aktiver/deaktiver

### ✅ Onboarding
- 3-slides introduksjon for nye brukere
- Checkout-mekanisme (vis maks 2 ganger)
- "Se introduksjon igjen" i innstillinger
- Keyboard shortcuts (←→ navigering, ESC lukk)

### ✅ AI Chat Assistant (mobil)
- Intelligent chatbot for ansatte
- 4 quick actions
- Demo-funksjon for dokumentopplasting
- Typing indicator

## 🎯 Roller

### 👨‍💼 Administrator
- Full tilgang til alle funksjoner
- API-administrasjon
- Alle kontrakter

### 📊 Prosjektleder
- Administrere bedrifter på egne kontrakter
- Registrere ansatte
- Eksportere rapporter

### 🏢 Underentreprenør
- Se egen bedrifts status
- Oversikt over ansatte
- Dokumentstatus

## 🧪 Innlogging (Demo)

Systemet har tre forhåndsvalgte roller:

- **Administrator**: Klikk på "Administrator"-kortet
- **Prosjektleder**: Klikk på "Prosjektleder"-kortet
- **Underentreprenør**: Klikk på "Underentreprenør"-kortet

## 📱 Mobil Upload

For ansatte som skal laste opp dokumenter:
- Åpne: `employee-upload-mobile.html`
- Gamifisert opplevelse
- Progress bar og confetti-animasjoner
- AI-assistent for hjelp

## 🗂️ Filstruktur

```
mesta-compliance/
├── index.html                          # Hovedapplikasjon
├── employee-upload-mobile.html         # Mobil opplastingsside
├── FINAL_IMPLEMENTATION_SUMMARY.md     # Komplett oversikt
├── DOCUMENT_REQUIREMENTS_GUIDE.md      # Guide til dokumentkrav
├── EXCEL_EXPORT_GUIDE.md              # Excel-export guide
├── IAM_CIAM_INTEGRATION_PLAN.md       # Fremtidig IAM-plan
└── README.md                          # Dette dokumentet
```

## 🎨 Design

- **Farger**: MESTA-palett (Oransje #FF6B35, Blå #004B87, Grønn #00A651)
- **Font**: Poppins (Google Fonts)
- **Animasjoner**: Smooth, moderne transitions
- **Responsivt**: Fungerer på desktop, tablet og mobil

## 🔧 Teknologi

- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **No dependencies**: Ingen eksterne libraries
- **API**: Brønnøysundregistrene (offentlig)
- **Storage**: LocalStorage for onboarding og preferanser

## 📊 Data

Systemet bruker mock-data for demonstrasjon:
- 3 forhåndsregistrerte bedrifter
- 9 bedrifter i søkedatabase
- All data forsvinner ved refresh
- Trygt å teste med

## 🧪 Testing

### Test 1: Legg til bedrift via søk
```
1. Logg inn som Admin
2. Klikk "➕ Legg til bedrift"
3. Søk på "Ps Anlegg" eller "912561798"
4. Velg bedrift fra resultatliste
5. Skriv inn kontrakt-ID
6. Velg dokumentkrav (3 forhåndsvalgt)
7. Klikk "✓ Bekreft og legg til"
8. Success! Bedrift er lagt til
```

### Test 2: Manuell registrering
```
1. Klikk "➕ Legg til bedrift"
2. Klikk "✏️ Registrer manuelt"
3. Fyll ut: Navn, Org.nr, Kontrakt-ID
4. Velg dokumentkrav
5. Bekreft
6. Ferdig!
```

### Test 3: Kontraktsfiltrering
```
1. Se dropdown "📋 Filtrer etter kontrakt"
2. Velg en kontrakt (f.eks. FV12-2025-MESTA)
3. Se at liste filtreres
4. Statistikk oppdateres
```

### Test 4: Excel-export
```
1. Åpne en bedrift
2. Scroll ned
3. Klikk "📊 Eksporter til Excel"
4. CSV lastes ned
5. Åpne i Excel
6. Se alle seksjoner
```

## 🎓 Dokumentasjon

Fullstendig dokumentasjon finnes i `/docs`:
- `FINAL_IMPLEMENTATION_SUMMARY.md` - Komplett oversikt over alle funksjoner
- `DOCUMENT_REQUIREMENTS_GUIDE.md` - Guide til dokumentkrav-systemet
- `EXCEL_EXPORT_GUIDE.md` - Alt om Excel-rapportering
- `IAM_CIAM_INTEGRATION_PLAN.md` - Plan for fremtidig IAM

## 🔮 Fremtidige forbedringer

### V2.1 (Neste sprint)
- [ ] Dokumentopplasting direkte i systemet
- [ ] Edit dokumentkrav etter registrering
- [ ] Push-notifikasjoner
- [ ] Offline mode

### V2.2 (Q2 2025)
- [ ] Template-profiler for dokumentkrav
- [ ] Bulk-operasjoner
- [ ] Historikk og audit trail
- [ ] Advanced analytics

### V3.0 (Q3 2025)
- [ ] Native mobile apps
- [ ] Altinn-integrasjon
- [ ] Biometric authentication
- [ ] AI-validering av dokumenter

## 📞 Support

For spørsmål eller problemer:
- Åpne et GitHub Issue
- Kontakt: [DIN E-POST]

## 📄 Lisens

Dette er en demo-applikasjon laget for MESTA.

---

**Laget med ❤️ for MESTA**

*Siste oppdatering: Februar 2025*
