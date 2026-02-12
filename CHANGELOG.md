# MESTA Compliance - Endringslogg
## Alle versjoner og oppdateringer

---

## [2.3.0] - 2025-02-12

### 🆕 Nye funksjoner
- **Compliance-visning for UE**: Underentreprenører ser nå påkrevd dokumentasjon med tydelig status
  - Grønn bakgrunn for OK dokumenter
  - Gul bakgrunn for manglende dokumenter
  - Rød bakgrunn for utløpte dokumenter
  - Advarsel-boks hvis noe mangler
  - Success-boks hvis alt er i orden

- **Klikk på ansatt for detaljer**: Ansatt-kort er nå klikkbare
  - Modal viser full informasjon
  - Kontaktinformasjon (e-post, telefon)
  - Alle dokumenter med status og utløpsdato
  - Beregner dager til utløp
  - Advarsler for dokumenter som snart utløper

- **Rollebasert sletting**: Forbedret tilgangskontroll
  - Kun Admin kan slette UE
  - Prosjektleder ser ikke slett-knapp lenger
  - Dobbel bekreftelse ved sletting

### 🎨 UI/UX forbedringer
- Pil-ikon (→) på klikkbare ansatt-kort
- Hover-effekt på ansatt-kort
- Excel-knapp tar full bredde når alene
- Forbedret layout i UE-visning

### 📚 Dokumentasjon
- ROLE_BASED_DELETE_RESTRICTION.md (tilgangskontroll)
- NEW_FEATURES_SPECIFICATION.md oppdatert
- README.md oppdatert med alle nye funksjoner

---

## [2.2.0] - 2025-02-11

### 🆕 Nye funksjoner
- **Dokumentkrav ved registrering**: 8 dokumenttyper å velge mellom
  - Skatteattest, MVA-attest, HMS-egenerklæring (forhåndsvalgt)
  - Forsikringsbevis, Ansatteliste, Kvalitetssertifikat
  - Miljøsertifikat, Sentral godkjenning
- **Validering**: Minst 1 dokument må velges
- **Success-melding**: Viser antall påkrevde dokumenter

### 📊 Excel-export
- Dokumentkrav inkludert i export
- Compliance-sjekker per bedrift

### 📚 Dokumentasjon
- DOCUMENT_REQUIREMENTS_GUIDE.md (komplett guide)

---

## [2.1.0] - 2025-02-10

### 🆕 Nye funksjoner
- **Kontraktsfiltrering**: Dropdown for å filtrere per kontrakt
- **Oversikts-export**: Excel-export respekterer valgt kontrakt
  - 7 seksjoner: Header, Sammendrag, Bedrifter, Compliance, Ansatte, Advarsler, Kritiske
  - Viser dokumenter som utløper snart (<30 dager)
  - Viser utløpte dokumenter

### 🐛 Feilrettinger
- Brønnøysund API søk med fallback til mock
- Bedre JSON-håndtering i søkeresultater
- Timeout på API-kall (3 sekunder)

### 📚 Dokumentasjon
- EXCEL_EXPORT_GUIDE.md (20+ sider)
- FINAL_IMPLEMENTATION_SUMMARY.md oppdatert

---

## [2.0.0] - 2025-02-09

### 🆕 Nye funksjoner
- **Onboarding**: 3-slides introduksjon
  - Checkout-mekanisme (vis maks 2 ganger)
  - "Se introduksjon igjen" i innstillinger
  - Keyboard shortcuts (←→, ESC)

- **Brønnøysund API**: Ekte søk i offentlige registre
  - Søk på org.nummer eller firmanavn
  - Fallback til mock ved API-feil

- **Manuell registrering**: 3 inngangspunkter
  - Direkte fra hovedmeny
  - Etter søk
  - Ved 0 søketreff

- **API-integrasjoner**: Panel for administrasjon
  - 4 integrasjoner (BrReg, StartBANK, Landax, HMSReg)
  - Test tilkobling
  - Synkroniser data
  - Aktiver/deaktiver

### 📱 Mobil
- employee-upload-mobile.html
  - Gamifisert opplastingsflyt
  - Progress bar og confetti
  - AI Chat Assistant

### 📚 Dokumentasjon
- FINAL_IMPLEMENTATION_SUMMARY.md
- IAM_CIAM_INTEGRATION_PLAN.md
- GITHUB_SETUP_GUIDE.md

---

## [1.0.0] - 2025-02-08

### 🎉 Initial Release
- Grunnleggende bedriftsadministrasjon
- Ansattregistrering
- Dokumentstatus
- 3 roller: Admin, Prosjektleder, UE
- Mock-database
- Responsive design

---

## 🔮 Planlagt (Fremtidige versjoner)

### [2.4.0] - Planlagt
- [ ] Sub-UE (underentreprenører til underentreprenører)
- [ ] Dokumentopplasting direkte i systemet
- [ ] Edit dokumentkrav etter registrering

### [2.5.0] - Q2 2025
- [ ] Bulk-operasjoner
- [ ] Historikk og audit trail
- [ ] Advanced analytics
- [ ] Push-notifikasjoner

### [3.0.0] - Q3 2025
- [ ] Native mobile apps (iOS/Android)
- [ ] Altinn-integrasjon
- [ ] Biometric authentication
- [ ] AI-validering av dokumenter
- [ ] IAM/CIAM (Auth0/Azure AD)

---

## 📝 Notater

### Versjonering
Vi følger [Semantic Versioning](https://semver.org/):
- **MAJOR** (X.0.0): Breaking changes
- **MINOR** (0.X.0): Nye funksjoner (bakoverkompatible)
- **PATCH** (0.0.X): Feilrettinger

### Tags
- 🆕 = Ny funksjon
- 🎨 = UI/UX forbedring
- 🐛 = Feilretting
- 📚 = Dokumentasjon
- 🔒 = Sikkerhet
- ⚡ = Ytelse
- 🔮 = Planlagt

---

*MESTA Compliance - Changelog*
*Siste oppdatering: 12. Februar 2025*
