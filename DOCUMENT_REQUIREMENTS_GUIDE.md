# MESTA Compliance - Dokumentkrav ved bedriftsregistrering
## Sjekkliste for påkrevd dokumentasjon

---

## 🎯 Ny funksjonalitet

Ved opprettelse av ny underentreprenør (UE) kan du nå velge hvilke dokumenter bedriften må levere for å være i compliance. Dette gir fleksibilitet til å tilpasse kravene per bedrift eller kontrakt.

---

## 📋 Tilgjengelige dokumenttyper

### **Standard dokumenter (forhåndsvalgt):**

#### **1. 🧾 Skatteattest**
- **Beskrivelse**: Bevis på innbetalt skatt
- **Formål**: Verifisere at bedriften har betalt skatt
- **Gyldighet**: Vanligvis 3-6 måneder
- **Kilde**: Skatteetaten

#### **2. 💰 MVA-attest**
- **Beskrivelse**: Merverdiavgift i orden  
- **Formål**: Bekrefte at MVA er betalt
- **Gyldighet**: Vanligvis 3 måneder
- **Kilde**: Skatteetaten

#### **3. 🦺 HMS-egenerklæring**
- **Beskrivelse**: Helse, miljø og sikkerhet
- **Formål**: Dokumentere HMS-rutiner
- **Gyldighet**: 12 måneder
- **Kilde**: Bedriften selv

### **Valgfrie dokumenter:**

#### **4. 🛡️ Forsikringsbevis**
- **Beskrivelse**: Ansvars- og yrkesskadeforsikring
- **Formål**: Verifisere forsikringsdekning
- **Gyldighet**: 12 måneder
- **Kilde**: Forsikringsselskap

#### **5. 👥 Ansatteliste**
- **Beskrivelse**: Oversikt over ansatte på prosjekt
- **Formål**: Kontrollere bemanning
- **Gyldighet**: Løpende oppdatert
- **Kilde**: Bedriften selv

#### **6. ⭐ Kvalitetssertifikat**
- **Beskrivelse**: ISO eller tilsvarende
- **Formål**: Verifisere kvalitetssystem
- **Gyldighet**: 36 måneder (avhengig av sertifikat)
- **Kilde**: Sertifiseringsorgan

#### **7. 🌱 Miljøsertifikat**
- **Beskrivelse**: Miljøledelsessystem
- **Formål**: Dokumentere miljøarbeid
- **Gyldighet**: 36 måneder
- **Kilde**: Sertifiseringsorgan

#### **8. 📜 Sentral godkjenning**
- **Beskrivelse**: For spesielle bransjer
- **Formål**: Verifisere autorisasjon
- **Gyldighet**: Varierer
- **Kilde**: Direktoratet for byggkvalitet

---

## 🔄 Brukerflyt

### **Metode 1: Via Proff.no søk**

```
1. Klikk "➕ Legg til bedrift"
   ↓
2. Søk på bedrift (navn eller org.nr)
   ↓
3. Velg bedrift fra resultatliste
   ↓
4. Skriv inn kontrakt-ID
   ↓
5. VELG DOKUMENTER (ny funksjonalitet!)
   ├─ ✓ Skatteattest (forhåndsvalgt)
   ├─ ✓ MVA-attest (forhåndsvalgt)
   ├─ ✓ HMS-egenerklæring (forhåndsvalgt)
   ├─ ☐ Forsikringsbevis
   ├─ ☐ Ansatteliste
   ├─ ☐ Kvalitetssertifikat
   ├─ ☐ Miljøsertifikat
   └─ ☐ Sentral godkjenning
   ↓
6. Klikk "✓ Bekreft og legg til"
   ↓
7. Success: "Bedrift AS er nå registrert - 3 dokumenter påkrevd"
```

### **Metode 2: Manuell registrering**

```
1. Klikk "➕ Legg til bedrift"
   ↓
2. Klikk "✏️ Registrer manuelt"
   ↓
3. Fyll ut:
   - Firmanavn
   - Org.nummer
   - Kontrakt-ID
   ↓
4. VELG DOKUMENTER (samme som over)
   ↓
5. Klikk "✓ Bekreft og legg til"
```

---

## 📊 Hvordan det vises i systemet

### **I bedriftsdetaljer:**

```
┌─────────────────────────────────────────────┐
│ 📋 Compliance-sjekker                       │
├─────────────────────────────────────────────┤
│ Skatteattest                    [⏳ Venter] │ ← Gul bakgrunn
│ Venter på dokumentasjon                     │
├─────────────────────────────────────────────┤
│ MVA-attest                      [⏳ Venter] │
│ Venter på dokumentasjon                     │
├─────────────────────────────────────────────┤
│ HMS-egenerklæring               [✓ OK]      │ ← Grønn bakgrunn
│ Sjekket: 09.02.2025 14:30                   │
└─────────────────────────────────────────────┘
```

### **Status-badges:**
- 🟢 **Grønn** = OK (dokument levert og godkjent)
- 🟡 **Gul** = VENTER (dokument ikke levert ennå)
- 🔴 **Rød** = EXPIRED/AVVIST (dokument utløpt eller avvist)

---

## 🎯 Bruksscenarioer

### **Scenario 1: Standard entreprenør**
```
Bedrift: Asfalt Service AS
Kontrakt: E18-2025-MESTA

Påkrevde dokumenter:
✓ Skatteattest
✓ MVA-attest
✓ HMS-egenerklæring

Rasjonale: Standard krav for alle entreprenører
```

### **Scenario 2: Større entreprenør med kvalitetskrav**
```
Bedrift: Veidrift Norge AS
Kontrakt: E6-2025-MESTA

Påkrevde dokumenter:
✓ Skatteattest
✓ MVA-attest
✓ HMS-egenerklæring
✓ Forsikringsbevis
✓ Kvalitetssertifikat (ISO 9001)
✓ Miljøsertifikat (ISO 14001)

Rasjonale: Større kontrakt krever mer omfattende dokumentasjon
```

### **Scenario 3: Spesialisert arbeid**
```
Bedrift: Elektro Spesialisten AS
Kontrakt: RV35-2025-MESTA

Påkrevde dokumenter:
✓ Skatteattest
✓ MVA-attest
✓ HMS-egenerklæring
✓ Forsikringsbevis
✓ Sentral godkjenning (Elektroentreprenør)

Rasjonale: Elektroarbeid krever sentral godkjenning
```

### **Scenario 4: Minimal dokumentasjon**
```
Bedrift: Liten Transport AS
Kontrakt: Kommunal-2025

Påkrevde dokumenter:
✓ Skatteattest
✓ MVA-attest

Rasjonale: Mindre kontrakt, minimale krav
```

---

## ⚙️ Teknisk implementering

### **Data-struktur:**

```javascript
const newUE = {
    id: 'ue-004',
    name: 'Bedrift AS',
    orgNumber: '123456789',
    contractId: 'FV12-2025-MESTA',
    status: 'ACTIVE',
    
    // Nye felter:
    requiredDocuments: [
        'TAX_CERTIFICATE',
        'VAT_CERTIFICATE',
        'HMS_DECLARATION',
        'INSURANCE_CERTIFICATE'
    ],
    
    complianceChecks: [
        {
            code: 'TAX_CERTIFICATE',
            name: 'Skatteattest',
            status: 'PENDING',  // eller 'OK', 'EXPIRED'
            icon: '⏳',          // eller '✓', '✗'
            checkedAt: '2025-02-11T10:00:00Z'
        },
        // ... mer checks
    ]
};
```

### **Validering:**

```javascript
// Minst 1 dokument må velges
if (selectedDocs.length === 0) {
    alert('⚠️ Vennligst velg minst ett dokument');
    return;
}

// Maks 8 dokumenter (alle tilgjengelige)
// Ingen maksgrense enforced
```

### **Success-melding:**

```javascript
`${companyName} er nå registrert i systemet
${selectedDocs.length} dokument${selectedDocs.length > 1 ? 'er' : ''} påkrevd`

// Eksempel output:
// "Bergvesen AS er nå registrert i systemet
//  3 dokumenter påkrevd"
```

---

## 🧪 Testing

### **Test 1: Standard valg (3 dokumenter)**
```
1. Legg til ny bedrift
2. La forhåndsvalgte stå (Skatteattest, MVA, HMS)
3. Bekreft
4. Resultat: 3 dokumenter påkrevd, alle status PENDING (gul)
```

### **Test 2: Alle dokumenter valgt**
```
1. Legg til ny bedrift
2. Huk av ALLE 8 checkboxes
3. Bekreft
4. Resultat: 8 dokumenter påkrevd
5. Åpne bedriftsdetaljer
6. Se alle 8 dokumenter listet under "Compliance-sjekker"
```

### **Test 3: Kun 1 dokument**
```
1. Legg til ny bedrift
2. Fjern alle unntatt "Skatteattest"
3. Bekreft
4. Resultat: 1 dokument påkrevd
```

### **Test 4: Ingen dokumenter (validering)**
```
1. Legg til ny bedrift
2. Fjern ALLE checkboxes
3. Klikk "Bekreft"
4. Resultat: Alert "⚠️ Vennligst velg minst ett dokument"
5. Kan ikke fortsette før minst 1 er valgt
```

### **Test 5: Manuell registrering**
```
1. Klikk "Registrer manuelt"
2. Fyll ut bedriftsinfo
3. Velg dokumenter (f.eks. 4 stk)
4. Bekreft
5. Resultat: Bedrift opprettet med 4 dokumenter
```

---

## 📊 Excel-export oppdatering

Dokumentkravene inkluderes automatisk i Excel-export:

### **Enkeltbedrift-export:**
```csv
COMPLIANCE-SJEKKER
Sjekk,Status,Tidspunkt
Skatteattest,PENDING,11.02.2025 10:00
MVA-attest,PENDING,11.02.2025 10:00
HMS-egenerklæring,OK,11.02.2025 10:00
Forsikringsbevis,PENDING,11.02.2025 10:00
```

### **Oversikts-export:**
```csv
BEDRIFTSOVERSIKT
Bedriftsnavn,Org.nr,Dokumenter totalt,Dokumenter OK,Dokumenter venter
Bergvesen AS,987654321,4,1,3
Anlegg Nord AS,876543210,3,3,0
```

---

## 💡 Best practices

### **For administratorer:**

1. **Standard-pakke**: Bruk forhåndsvalgte (3 dok) for de fleste
2. **Større kontrakter**: Legg til Forsikring + Kvalitet/Miljø
3. **Spesialarbeid**: Legg til Sentral godkjenning når relevant
4. **Konsistens**: Bruk samme dokumentkrav for samme type kontrakt

### **For prosjektledere:**

1. **Vær spesifikk**: Velg kun dokumenter du faktisk trenger
2. **Ikke overdriv**: Flere dokumenter = mer arbeid for UE
3. **Følg opp**: Sjekk at pending-dokumenter leveres
4. **Kommuniser**: Fortell UE hvilke dokumenter som kreves

### **Anbefalte kombinasjoner:**

```
Minimal (små kontrakter):
  ✓ Skatteattest
  ✓ MVA-attest

Standard (vanlige entreprenører):
  ✓ Skatteattest
  ✓ MVA-attest
  ✓ HMS-egenerklæring

Omfattende (store/kritiske kontrakter):
  ✓ Skatteattest
  ✓ MVA-attest
  ✓ HMS-egenerklæring
  ✓ Forsikringsbevis
  ✓ Kvalitetssertifikat
  ✓ Miljøsertifikat

Spesialisert (fagbransjer):
  ✓ Alle standard +
  ✓ Sentral godkjenning
```

---

## 🔮 Fremtidige forbedringer

### **V2.1:**
- [ ] Sett utløpsdato per dokument
- [ ] Automatisk varsling før utløp
- [ ] Last opp dokumenter direkte i systemet
- [ ] OCR-scanning av dokumenter

### **V2.2:**
- [ ] Template-profiler (spar dokumentvalg)
- [ ] Bulk-oppdatering av dokumentkrav
- [ ] Historikk over dokumentendringer
- [ ] Godkjenningsflyt for dokumenter

### **V3.0:**
- [ ] Integrasjon mot Altinn
- [ ] Automatisk henting fra offentlige registre
- [ ] Digital signering av dokumenter
- [ ] AI-validering av dokumentinnhold

---

## 📞 Support

### **Vanlige spørsmål:**

**Q: Kan jeg endre dokumentkrav etter registrering?**
A: I V2.0 må du oppdatere manuelt i databasen. V2.1 vil ha edit-funksjon.

**Q: Hva skjer hvis jeg ikke velger noen dokumenter?**
A: Du får en feilmelding og må velge minst 1 dokument.

**Q: Kan jeg legge til egne dokumenttyper?**
A: Ikke i V2.0. Bruk de 8 tilgjengelige typene. Tilpasning kommer i V2.2.

**Q: Hvor ser jeg hvilke dokumenter som er påkrevd?**
A: Åpne bedriftsdetaljer → Se "Compliance-sjekker" seksjonen.

**Q: Hvordan oppdaterer jeg status fra PENDING til OK?**
A: Manuelt i V2.0. V2.1 vil ha upload + godkjenning direkte i UI.

---

## ✅ Sjekkliste for produksjon

- [x] Dokumentvalg i søkeflyt
- [x] Dokumentvalg i manuell registrering
- [x] Validering (minst 1 dokument)
- [x] Success-melding viser antall
- [x] Compliance-sjekker viser riktig status
- [x] Farger: Grønn (OK), Gul (PENDING), Rød (ERROR)
- [x] Excel-export inkluderer dokumenter
- [ ] Dokumentopplasting (kommer i V2.1)
- [ ] Edit dokumentkrav (kommer i V2.1)
- [ ] Automatisk status-oppdatering (kommer i V2.1)

---

**MESTA Compliance - Dokumentkrav implementert og produksjonsklart!**

*Siste oppdatering: 11. Februar 2025*
