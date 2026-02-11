# MESTA Compliance - Excel Export Guide
## Komplett guide til eksportfunksjoner

---

## 📊 To typer Excel-export

### 1️⃣ **Oversiktsrapport** (Ny!)
**Hvor**: Hovedoversikten
**Hva**: Samlet rapport over alle filtrerte bedrifter
**Bruk**: Månedlig rapportering, presentasjoner, analyse

### 2️⃣ **Enkeltbedrift**
**Hvor**: Bedriftsdetaljer-modal
**Hva**: Detaljert rapport for én spesifikk bedrift
**Bruk**: Deling med underentreprenør, dokumentasjon

---

## 📋 Oversiktsrapport - Komplett guide

### **Plassering:**
```
┌─────────────────────────────────────────┐
│ 🏢 Registrerte bedrifter                │
├─────────────────────────────────────────┤
│ 📋 Filtrer: [FV12-2025 ▼]               │
│           [📊 Eksporter oversikt] ←──   │
├─────────────────────────────────────────┤
│ Viser 2 bedrift(er) på kontrakt...     │
└─────────────────────────────────────────┘
```

### **Flyt:**
```
1. Velg kontrakt (eller "Alle kontrakter")
2. Klikk "📊 Eksporter oversikt til Excel"
3. Loading: "Genererer Excel-rapport..."
4. Fil lastes ned automatisk
5. Success: "✓ Excel-rapport lastet ned: X bedrift(er)"
```

### **Filnavn:**
- **Alle kontrakter**: `MESTA_Oversikt_Alle_20250211.csv`
- **Én kontrakt**: `MESTA_Oversikt_FV12_2025_MESTA_20250211.csv`

---

## 📄 Rapportinnhold - 7 seksjoner

### **Seksjon 1: Header**
```
MESTA COMPLIANCE - SAMLET OVERSIKT

Rapport generert: 11.02.2025 10:45
Filter: FV12-2025-MESTA
Antall bedrifter: 2
```

### **Seksjon 2: Sammendrag**
```
SAMMENDRAG
Bedrifter totalt          2
Godkjente bedrifter       1
Sperrede bedrifter        1
Totalt ansatte            3
Totalt dokumenter         9
Dokumenter OK             7
Dokumenter utløpt         1
Dokumenter mangler        1
```

### **Seksjon 3: Bedriftsoversikt (hovedtabell)**
```
BEDRIFTSOVERSIKT
Bedriftsnavn      | Org.nr    | Kontrakt       | Status   | Ansatte | Dok totalt | Dok OK | Dok utløpt | Sist sjekket
Bergvesen AS      | 987654321 | FV12-2025      | Godkjent | 2       | 6          | 5      | 1          | 09.02 14:30
Anlegg Nord AS    | 876543210 | FV12-2025      | Sperret  | 1       | 3          | 2      | 0          | 08.02 10:15
```

### **Seksjon 4: Compliance-sjekker per bedrift**
```
COMPLIANCE-SJEKKER PER BEDRIFT
Bedriftsnavn      | Sjekk                    | Status  | Tidspunkt
Bergvesen AS      | Aktivt i Brønnøysund    | OK      | 09.02 14:30
                  | HMS-egenerklæring        | OK      | 09.02 14:30
                  | Skatteattest             | OK      | 09.02 14:30
Anlegg Nord AS    | Aktivt i Brønnøysund    | OK      | 08.02 10:15
                  | HMS-egenerklæring        | EXPIRED | 08.02 10:15
                  | Skatteattest             | OK      | 08.02 10:15
```

### **Seksjon 5: Ansatte og dokumenter - detaljert**
```
ANSATTE OG DOKUMENTER - DETALJERT
Bedrift       | Ansatt      | Stilling         | Telefon        | E-post              | Dokument           | Status  | Utløpsdato
Bergvesen AS  | Per Hansen  | Gravemaskinfører | +47 900 00 001 | per@bergvesen.no    | Førerkort          | OK      | 15.05.2026
              |             |                  |                |                     | Maskinførerbevis   | OK      | 20.03.2027
              |             |                  |                |                     | HMS-opplæring      | OK      | 10.06.2026
Bergvesen AS  | Kari Olsen  | Anleggsleder     | +47 900 00 002 | kari@bergvesen.no   | Førerkort          | OK      | 10.02.2027
              |             |                  |                |                     | HMS-opplæring      | EXPIRED | 15.01.2025
              |             |                  |                |                     | Fagbrev            | OK      | Ingen
Anlegg Nord AS| Ole J.      | Tømrer           | +47 900 00 003 | ole@anleggnord.no   | Førerkort          | OK      | 10.02.2027
              |             |                  |                |                     | Fagbrev tømrer     | OK      | Ingen
              |             |                  |                |                     | HMS-opplæring      | OK      | 18.06.2026
```

### **Seksjon 6: Advarsler - Dokumenter som utløper snart**
```
ADVARSEL - DOKUMENTER SOM UTLØPER SNART (< 30 DAGER)
Bedrift       | Ansatt      | Dokument      | Utløpsdato      | Dager igjen
Bergvesen AS  | Kari Olsen  | HMS-kurs      | 15.03.2025      | 22
```

### **Seksjon 7: Kritiske - Utløpte dokumenter**
```
KRITISK - UTLØPTE DOKUMENTER
Bedrift       | Ansatt      | Dokument      | Utløpt dato
Bergvesen AS  | Kari Olsen  | HMS-opplæring | 15.01.2025
```

---

## 🔍 Eksempler på bruk

### **Scenario 1: Månedlig rapportering til prosjektleder**
```
Prosjektleder ønsker oversikt over FV12-prosjektet:

1. Velg "FV12-2025-MESTA" i dropdown
2. Klikk "Eksporter oversikt"
3. Åpne CSV i Excel
4. Se:
   - 2 bedrifter på FV12
   - 1 godkjent, 1 sperret
   - 3 ansatte totalt
   - 1 dokument utløpt (kritisk!)
5. Send rapporten til kunde
```

### **Scenario 2: Kontrakt-audit**
```
Revisor ønsker dokumentasjon for hele kontrakten:

1. Velg "E18-2025-MESTA"
2. Eksporter oversikt
3. CSV inneholder:
   - Alle bedrifter på E18
   - Alle compliance-sjekker
   - Alle ansatte og dokumenter
   - Advarsler om utløp
4. Bruk som audit trail
```

### **Scenario 3: Sammenligning på tvers**
```
Leder ønsker sammenligne alle kontrakter:

1. Velg "Alle kontrakter"
2. Eksporter oversikt
3. Pivot-analyse i Excel:
   - Bedrifter per kontrakt
   - Compliance-rate per kontrakt
   - Dokumentutløp per kontrakt
4. Identifiser problemområder
```

### **Scenario 4: Varsling om utløp**
```
HMS-ansvarlig sjekker dokumenter månedlig:

1. Velg "Alle kontrakter"
2. Eksporter
3. Gå til seksjon "ADVARSEL - DOKUMENTER SOM UTLØPER SNART"
4. Se liste over dokumenter < 30 dager
5. Send purring til berørte UE
```

---

## 📊 Enkeltbedrift-export

### **Plassering:**
```
Åpne bedrift → Scroll ned:
┌─────────────────────────────┐
│ [➕ Legg til ansatt]        │
│ [📊 Eksporter til Excel]    │
└─────────────────────────────┘
```

### **Innhold:**
```
Seksjon 1: Bedriftsinformasjon
Seksjon 2: Compliance-sjekker
Seksjon 3: Ansatte og dokumenter (detaljert)
Seksjon 4: Statistikk
```

### **Bruksområde:**
- Dele med underentreprenør
- Dokumentasjon til kunde
- Arkivering
- Kvalitetskontroll

---

## 🎯 Sammenligning: Oversikt vs. Enkelt

| Feature | Oversiktsrapport | Enkeltbedrift |
|---------|------------------|---------------|
| **Antall bedrifter** | Mange (filtrert) | Én |
| **Sammendrag** | ✅ Ja | ✅ Ja (én bedrift) |
| **Compliance** | ✅ Alle bedrifter | ✅ Én bedrift |
| **Ansatte** | ✅ Alle | ✅ Én bedrift |
| **Advarsler** | ✅ På tvers | ❌ Nei |
| **Kritiske utløp** | ✅ På tvers | ❌ Nei |
| **Filtrering** | ✅ Per kontrakt | ❌ N/A |
| **Beste for** | Rapportering, audit | Deling, dokumentasjon |

---

## 📱 Excel-tips

### **Åpne CSV i Excel:**
```
1. Høyreklikk på CSV-fil
2. Velg "Åpne med → Excel"
   ELLER
3. I Excel: File → Open → Velg CSV
4. Excel åpner automatisk med riktig formatering
```

### **Norske tegn (æøå):**
```
✅ Fungerer automatisk!
CSV-filen har UTF-8 BOM encoding
Excel tolker dette korrekt
```

### **Lag pivot-tabell:**
```
1. Åpne CSV i Excel
2. Merk dataområdet
3. Insert → PivotTable
4. Dra felter til Rows/Columns/Values
5. Eksempel:
   - Rows: Kontrakt
   - Values: Antall bedrifter, Sum ansatte
```

### **Filtrere i Excel:**
```
1. Klikk på header-rad
2. Data → Filter
3. Se dropdown-piler på hver kolonne
4. Filtrer på Status, Kontrakt, etc.
```

### **Fargekoding:**
```
Conditional formatting:
- Grønn: Status = "OK"
- Rød: Status = "EXPIRED"
- Gul: Dager igjen < 30
```

---

## 🔐 Sikkerhet og personvern

### **Dataansvar:**
```
⚠️ Eksporterte filer inneholder:
- Personnavn
- Telefonnummer
- E-postadresser
- Organisasjonsnummer

Håndtering:
✅ Del kun over sikre kanaler
✅ Slett filer etter bruk
✅ Ikke send på usikret e-post
✅ Ikke lagre på usikrede enheter
```

### **Audit trail:**
```
I produksjon vil eksport logges:
- Hvem eksporterte
- Når (timestamp)
- Hvilke data (kontrakt/bedrift)
- Fra hvilken IP-adresse

Dette for GDPR compliance og sikkerhet.
```

---

## 🚀 Fremtidige forbedringer

### **V2.1 - Excel-bibliotek:**
```
Erstatt CSV med ekte Excel (.xlsx):
- Multi-sheet (ark per bedrift)
- Formatering (farger, borders)
- Formler (auto-sum)
- Grafer (compliance-rate)
- Logo og header
```

### **V2.2 - Scheduled exports:**
```
Automatisk månedlig eksport:
- Hver 1. i måneden
- E-post til prosjektleder
- Attachment: Oversiktsrapport
- Summering av endringer
```

### **V2.3 - Custom templates:**
```
Brukerdefinerte maler:
- Velg hvilke kolonner
- Velg sorteringsrekkefølge
- Lagre som template
- Gjenbruk senere
```

---

## 🧪 Testing-sjekkliste

### **Test oversiktsrapport:**
- [ ] Eksporter "Alle kontrakter" → CSV med alle 3 bedrifter
- [ ] Eksporter "FV12-2025" → CSV med 2 bedrifter
- [ ] Eksporter "E18-2025" → CSV med 1 bedrift
- [ ] Åpne i Excel → Norske tegn vises korrekt
- [ ] Sjekk summering → Tall stemmer
- [ ] Sjekk advarsler → Dokumenter < 30 dager vises
- [ ] Sjekk kritiske → Utløpte dokumenter vises

### **Test enkeltbedrift:**
- [ ] Eksporter Bergvesen AS → CSV med 2 ansatte
- [ ] Eksporter Anlegg Nord AS → CSV med 1 ansatt
- [ ] Åpne i Excel → Formatering OK
- [ ] Sjekk compliance → Alle sjekker vises
- [ ] Filnavn → Inneholder bedriftsnavn

### **Edge cases:**
- [ ] Eksporter bedrift uten ansatte → Vis "Ingen ansatte"
- [ ] Eksporter bedrift uten compliance → Vis "Ingen sjekker"
- [ ] Kontrakt uten bedrifter → Vis advarsel før eksport
- [ ] Spesialtegn i navn → Filnavn saniteres

---

## 💡 Pro tips

### **Tip 1: Sammenlign måneder**
```
1. Eksporter oversikt hver måned
2. Lagre med måned i filnavn
3. Sammenlign:
   - MESTA_Oversikt_Alle_202501.csv
   - MESTA_Oversikt_Alle_202502.csv
4. Se utvikling over tid
```

### **Tip 2: Del med kunde**
```
1. Eksporter oversikt for kundens kontrakt
2. Fjern sensitive kolonner (telefon, e-post)
3. Konverter til PDF
4. Send til kunde
```

### **Tip 3: Print-vennlig**
```
1. Åpne CSV i Excel
2. Page Layout → Orientation: Landscape
3. Scale to fit: 1 page wide
4. Print eller lagre som PDF
```

### **Tip 4: Dashboard i Excel**
```
1. Eksporter "Alle kontrakter"
2. Lag pivot-tabeller
3. Lag grafer:
   - Compliance-rate per kontrakt
   - Ansatte per bedrift
   - Dokumentutløp timeline
4. Oppfrisk månedlig
```

---

## 📞 Support

### **Vanlige spørsmål:**

**Q: Hvorfor CSV og ikke Excel?**
A: CSV er universelt, lett, og åpnes i Excel. V2.1 vil ha .xlsx support.

**Q: Kan jeg eksportere til PDF?**
A: Åpne CSV i Excel, deretter File → Save As → PDF.

**Q: Norske tegn vises feil?**
A: Åpne direkte i Excel (ikke Notepad). CSV har UTF-8 BOM.

**Q: Kan jeg velge hvilke kolonner?**
A: Ikke i V2.0. V2.3 vil ha custom templates.

**Q: Hvor lagres eksporten?**
A: I nettleserens standard nedlastingsmappe (vanligvis "Downloads").

---

## 🎯 Konklusjon

### **Oversiktsrapport = Kraftig verktøy**
- ✅ Respekterer filtrering
- ✅ 7 seksjoner med all data
- ✅ Advarsler og kritiske punkter
- ✅ Excel-kompatibel
- ✅ Klar for rapportering

### **Enkeltbedrift = Enkel deling**
- ✅ Kompakt format
- ✅ Alle detaljer for én bedrift
- ✅ Ideell for å sende til UE

**Sammen gir de komplett eksportfunksjonalitet!**

---

*MESTA Compliance - Excel Export Guide*
*Februar 2025*
