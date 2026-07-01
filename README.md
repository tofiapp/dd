# Fotky na A4

Jednostránková webová aplikace (jen HTML/CSS/JS, žádný server ani build).
Nahraješ fotky po událostech a ona je automaticky rozvrhne na stránky A4
k tisku – s automatickou orientací na výšku i na šířku.

## Nasazení na Netlify – 3 způsoby

### 1) Nejrychleji: přetažením (Netlify Drop)
1. Otevři https://app.netlify.com/drop
2. Přetáhni sem **celou tuto složku** (nebo přiložený soubor
   `fotky-a4-netlify.zip`).
3. Hotovo – Netlify ti během chvilky vytvoří veřejnou adresu.

### 2) Přes Git (automatické aktualizace)
1. Nahraj obsah složky do repozitáře na GitHub/GitLab.
2. Na Netlify: **Add new site → Import an existing project**, vyber repozitář.
3. Build command nech prázdný, **Publish directory** nastav na `.`.

### 3) Přes Netlify CLI
```bash
npm install -g netlify-cli
netlify deploy --dir=. --prod
```

## Soubory
- `index.html` – celá aplikace
- `netlify.toml` – konfigurace (publish = ".", přesměrování na index.html)
