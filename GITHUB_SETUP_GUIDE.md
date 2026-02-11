# MESTA Compliance - GitHub Pages Oppsett
## Steg-for-steg guide for deling med kollegaer

---

## 📦 Hva du trenger å laste opp

Du har fått følgende filer som skal lastes opp til GitHub:

### **Essensielle filer (MÅ lastes opp):**
1. ✅ **index.html** - Hovedapplikasjonen (137 KB)
2. ✅ **README.md** - Beskrivelse av prosjektet

### **Ekstra filer (valgfritt, men anbefalt):**
3. ⭐ **employee-upload-mobile.html** - Mobil opplastingsside
4. 📄 **FINAL_IMPLEMENTATION_SUMMARY.md** - Komplett dokumentasjon
5. 📄 **DOCUMENT_REQUIREMENTS_GUIDE.md** - Guide til dokumentkrav
6. 📄 **EXCEL_EXPORT_GUIDE.md** - Excel-export guide
7. 📄 **IAM_CIAM_INTEGRATION_PLAN.md** - Fremtidig IAM-plan

---

## 🚀 Steg 1: Opprett GitHub-konto

### **Hvis du IKKE har GitHub-konto:**

1. Gå til: **https://github.com**
2. Klikk **"Sign up"** (øverst til høyre)
3. Fyll ut:
   - E-post: `din@epost.no`
   - Passord: (velg et sterkt passord)
   - Username: `mestauser` (eller noe annet)
4. Verifiser e-post (sjekk innboks)
5. Du er nå innlogget!

### **Hvis du HAR GitHub-konto:**

1. Gå til: **https://github.com**
2. Klikk **"Sign in"**
3. Logg inn
4. Du er klar!

---

## 🗂️ Steg 2: Opprett nytt repository

1. **Klikk på "+" ikonet** øverst til høyre
2. Velg **"New repository"**

3. **Fyll ut skjema:**
   ```
   Repository name: mesta-compliance
   Description: MESTA Compliance System - Demo
   
   ⚪ Public  ← Velg denne!
   ⚪ Private
   
   ☐ Add a README file  ← IKKE huk av (vi laster opp egen)
   ☐ Add .gitignore
   ☐ Choose a license
   ```

4. **Klikk "Create repository"** (grønn knapp nederst)

5. Du kommer til et nytt repository! 🎉

---

## 📤 Steg 3: Last opp filene

Du er nå på repository-siden og ser instruksjoner.

### **Metode A: Via nettleser (enklest)**

1. **Klikk "uploading an existing file"** (midt på siden)
   
2. **Dra filene inn i boksen:**
   - Dra **index.html** inn
   - Dra **README.md** inn
   - (Valgfritt) Dra resten av filene inn

3. **Vent til opplasting er ferdig** (grønn hake)

4. **Scroll ned og klikk "Commit changes"** (grønn knapp)

5. Filene er nå lastet opp! ✅

---

## 🌐 Steg 4: Aktiver GitHub Pages

1. **Klikk på "Settings"** (øverst, siste fane)

2. **Scroll ned til "Pages"** (venstre meny)

3. **Under "Source" (midt på siden):**
   ```
   Source: Deploy from a branch
   Branch: main  ← Velg fra dropdown
   Folder: / (root)  ← Velg fra dropdown
   ```

4. **Klikk "Save"** (blå knapp)

5. **Vent 1-2 minutter** (GitHub bygger siden)

6. **Refresh siden**

7. Du ser nå en blå boks øverst:
   ```
   🌐 Your site is live at https://[ditt-brukernavn].github.io/mesta-compliance/
   ```

8. **Kopier linken!** Dette er din offentlige URL! 🎉

---

## 🎯 Steg 5: Test at det fungerer

1. **Åpne linken** i ny fane:
   ```
   https://[ditt-brukernavn].github.io/mesta-compliance/
   ```

2. **Du skal se:**
   - Login-skjermen med 3 roller
   - MESTA logo og design
   - Onboarding starter automatisk

3. **Test innlogging:**
   - Klikk "Administrator"
   - Se dashboard
   - Alt fungerer! ✅

---

## 📧 Steg 6: Del med kollegaer

### **Send denne meldingen:**

```
Hei!

Jeg har satt opp en demo av MESTA Compliance-systemet.

🔗 Link: https://[ditt-brukernavn].github.io/mesta-compliance/

📱 Åpne på PC, Mac eller mobil - fungerer overalt!

🔐 Innlogging (demo):
• Administrator: Klikk "Administrator"
• Prosjektleder: Klikk "Prosjektleder"  
• Underentreprenør: Klikk "Underentreprenør"

✨ Test gjerne:
✓ Legg til bedrift (søk "Ps Anlegg" eller "912561798")
✓ Velg dokumentkrav (8 typer tilgjengelig)
✓ Filtrer per kontrakt
✓ Eksporter til Excel
✓ Se onboarding-intro (første gang)

💾 Data:
All data er mock-data og forsvinner ved refresh.
Trygt å teste alt!

🙌 Gi gjerne feedback!
```

---

## 🔧 Ekstra: Hvis du vil oppdatere senere

### **Legge til nye filer:**

1. Gå til repository: `https://github.com/[ditt-brukernavn]/mesta-compliance`
2. Klikk "Add file" → "Upload files"
3. Dra inn nye filer
4. Commit changes
5. Venter 1-2 min
6. Endringer er live!

### **Endre eksisterende fil:**

1. Gå til repository
2. Klikk på filen (f.eks. `index.html`)
3. Klikk på blyant-ikonet (Edit)
4. Gjør endringer
5. Scroll ned
6. Klikk "Commit changes"
7. Venter 1-2 min
8. Endringer er live!

---

## 🎨 Ekstra: Custom URL (valgfritt)

Hvis du vil ha en finere URL:

### **Uten custom domain:**
```
https://brukernavn.github.io/mesta-compliance/
```

### **Med custom domain (krever domene):**
```
https://mestacompliance.no
```

**Slik setter du det opp:**

1. Kjøp domene (f.eks. på `domeneshop.no` - ~100 kr/år)
2. Gå til Settings → Pages
3. Under "Custom domain" skriv: `mestacompliance.no`
4. Klikk "Save"
5. Følg instruksjonene for DNS-oppsett
6. Vent 24 timer
7. Ferdig!

---

## 🐛 Feilsøking

### **"I can't see the repository"**
→ Sjekk at du er innlogget på GitHub

### **"Upload button is disabled"**
→ Sjekk at du har valgt riktig repository
→ Prøv å laste opp én fil om gangen

### **"The site is not loading"**
→ Vent 2-3 minutter etter å ha aktivert Pages
→ Refresh siden
→ Sjekk at URL er riktig (github.io, ikke github.com)

### **"I get a 404 error"**
→ Sjekk at filen heter **index.html** (ikke ue-compliance-complete-v2.html)
→ Sjekk at Pages er aktivert i Settings

### **"Some features don't work"**
→ Normal! Brønnøysund API kan være blokkert (CORS)
→ Fallback til mock-data fungerer automatisk
→ Alt annet skal fungere perfekt

### **"Onboarding doesn't show"**
→ Åpne i inkognito/privat vindu
→ Eller: F12 → Application → Local Storage → Clear

---

## 📊 Oversikt over hva som skjer

```
Din PC
  ↓ (upload)
GitHub.com
  ↓ (deploy)
GitHub Pages Server
  ↓ (serve)
https://[brukernavn].github.io/mesta-compliance/
  ↓ (access)
Kollegaer verden over! 🌍
```

---

## ✅ Sjekkliste

Før du deler med kollegaer, sjekk:

- [ ] Repository er opprettet
- [ ] index.html er lastet opp
- [ ] README.md er lastet opp
- [ ] GitHub Pages er aktivert
- [ ] Linken fungerer (du kan åpne den selv)
- [ ] Onboarding vises første gang
- [ ] Innlogging fungerer
- [ ] Kan legge til bedrift
- [ ] Kan eksportere til Excel

Hvis alle er ✅, er du klar til å dele! 🎉

---

## 🎯 Forventet resultat

Din kollega vil:

1. **Klikke på linken**
2. **Se MESTA Compliance login-skjerm**
3. **Se onboarding automatisk** (3 slides)
4. **Kunne teste alt:**
   - Legge til bedrifter
   - Velge dokumentkrav
   - Filtrere per kontrakt
   - Eksportere til Excel
   - API-integrasjoner
5. **Data forsvinner ved refresh** (trygt å teste)

---

## 💡 Pro tips

### **Tip 1: Bruk kort URL**
Hvis GitHub-URL er for lang, bruk URL-shortener:
- bit.ly
- tinyurl.com

### **Tip 2: QR-kode**
Generer QR-kode av linken:
- qr-code-generator.com
- Skriv ut og sett opp på kontoret

### **Tip 3: Bookmark**
Be kollegaer bookmarke linken for enkel tilgang

### **Tip 4: Analytics**
Hvis du vil spore besøk:
- Google Analytics (gratis)
- Legg til tracking-kode i index.html

---

## 🎓 Video-tutorial (anbefalt)

Hvis du foretrekker video, se:
- GitHub Pages Tutorial: https://www.youtube.com/watch?v=QyFcl_Fba-k
- (Søk på "GitHub Pages tutorial" på YouTube)

---

## 📞 Trenger du hjelp?

Hvis du sitter fast:

1. **Google søk**: "GitHub pages not working"
2. **GitHub Docs**: https://docs.github.com/en/pages
3. **Stack Overflow**: Søk på feilmelding
4. **Spør meg**: Jeg kan hjelpe videre!

---

## 🎉 Gratulerer!

Når du har kommet så langt, har du:
- ✅ Opprettet GitHub-konto
- ✅ Opprettet repository
- ✅ Lastet opp filer
- ✅ Aktivert GitHub Pages
- ✅ Fått en fungerende live demo
- ✅ Delt med kollegaer

**Du er nå en GitHub Pages-ekspert!** 🚀

---

*MESTA Compliance - GitHub Pages Guide*
*Februar 2025*
