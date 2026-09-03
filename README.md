# QualitySteel

Skill Claude per estrarre dati da certificati materiale (forgia e/o
acciaieria) di prodotti metallici — tondi, gomiti, tubi, barre — presenti
in PDF, generando una scheda PDF riepilogativa per ogni Heat/Colata trovata.

## Contenuto

- `SKILL.md` — istruzioni e regole di estrazione (identificazione pagine,
  disambiguazione forgia/acciaieria, gestione campioni multipli, priorità
  tra fonti, ecc.).
- `scripts/genera_scheda_heat.py` — script Python che genera la scheda PDF
  a partire da un dizionario di dati estratti.

## Come pubblicarla su GitHub

Dal tuo terminale, nella cartella che contiene questa `quality-steel/`:

```bash
cd quality-steel
git init
git add .
git commit -m "Prima versione skill QualitySteel"
git branch -M main
git remote add origin https://github.com/<tuo-utente>/<tuo-repo>.git
git push -u origin main
```

Se il repository non esiste ancora, crealo prima su github.com (pulsante
"New repository"), poi usa l'URL che ti fornisce GitHub al posto di
`<tuo-utente>/<tuo-repo>`.

## Come reinstallarla su Claude

Su claude.ai/Cowork, carica il file `.skill` generato con `package_skill.py`
(oppure l'intera cartella se il tuo ambiente supporta skill locali) tramite
il pulsante "Save skill"/gestione skill.
