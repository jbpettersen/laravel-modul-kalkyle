# 🚀 Laravel Docker Template – Gjenbruksguide

Denne guiden forklarer hvordan du bruker dette repoet som utgangspunkt for nye prosjekter, f.eks. kalkyler, API-tjenester, datavisualisering osv.

---

## 🧱 1. Klon eksisterende prosjekt

```bash
git clone https://github.com/jbpettersen/laravel-modul-kalkyle.git mitt-nye-prosjekt
cd mitt-nye-prosjekt
```

---

## 🔄 2. Fjern tilknytning til originalt repo

```bash
git remote remove origin
```

---

## 📦 3. Start et nytt Git-repo

```bash
git init
git remote add origin https://github.com/dittbrukernavn/min-nye-app.git
git add .
git commit -m "Initial commit basert på Laravel template"
git push -u origin main
```

---

## 🧼 4. Tilpass til ditt nye prosjekt

- Rediger `README.md`
- Gi nytt navn til moduler, namespace osv.
- Fjern evt. gamle domenespesifikke komponenter (eks. `AnnualCalculation`)
- Oppdater `.env` om nødvendig

---

## 🐳 5. Start utvikling

```bash
docker-compose up -d
```

Hvis Laravel ikke er installert ennå:

```bash
docker-compose run --rm app composer create-project laravel/laravel .
```

---

## 🧠 Tips

- Hold denne mappen ren og modulær for maksimal gjenbruk
- Bruk gjerne `main` som base-template-bransje
- Du kan lage flere maler for ulike bruksområder senere (f.eks. `template-kalkyle`, `template-api`, osv.)

Lykke til! 🎉
