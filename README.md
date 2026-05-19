# Ildavini – Sito Web Ufficiale
### Cantina d'Abruzzo · Dal 1962

Sito web statico costruito con **[Astro](https://astro.build)** — framework moderno per siti ad alte prestazioni.

---

## 🚀 Avvio rapido

### 1. Installa le dipendenze
```bash
npm install
```

### 2. Avvia in modalità sviluppo
```bash
npm run dev
```
Il sito sarà disponibile su **http://localhost:4321**

### 3. Build per produzione
```bash
npm run build
```
I file statici vengono generati nella cartella `dist/`.

### 4. Anteprima del build
```bash
npm run preview
```

---

## 📁 Struttura del progetto

```
ildavini/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Nav.astro         # Navigazione principale
│   │   ├── Hero.astro        # Sezione hero / copertina
│   │   ├── Storia.astro      # Storia della cantina
│   │   ├── Vini.astro        # Menù dei vini
│   │   ├── Gallery.astro     # Galleria fotografica
│   │   ├── Video.astro       # Sezione video YouTube
│   │   ├── Contatti.astro    # Contatti + mappa + WhatsApp
│   │   ├── SocialBar.astro   # Barra social media
│   │   └── Footer.astro      # Piè di pagina
│   ├── layouts/
│   │   └── BaseLayout.astro  # Layout HTML base
│   ├── pages/
│   │   └── index.astro       # Pagina principale
│   └── styles/
│       └── global.css        # Variabili CSS e stili globali
├── astro.config.mjs
└── package.json
```

---

## ✏️ Personalizzazioni

### Numero WhatsApp
In `src/components/Contatti.astro`, riga 2:
```js
const WHATSAPP_NUMBER = '39085123456'; // ← Inserisci il tuo numero (con prefisso)
```

### Video YouTube
In `src/components/Video.astro`, sostituisci l'ID del video nell'URL:
```html
src="https://www.youtube.com/embed/IL_TUO_ID_VIDEO?rel=0"
```

### Link social media
In `src/components/SocialBar.astro`, aggiorna i link `href` di Instagram e Facebook.

### Vini nel menù
In `src/components/Vini.astro`, modifica l'array `vini` aggiungendo, rimuovendo o modificando le etichette.

### Colori del sito
In `src/styles/global.css`, modifica le variabili CSS:
```css
:root {
  --burgundy:   #5B1A1A;
  --gold:       #C8A96E;
  /* ... */
}
```

### Informazioni di contatto
In `src/components/Contatti.astro`, aggiorna l'array `contactItems` con indirizzo, telefono ed email reali.

---

## 🌐 Deploy

Il sito produce file statici. Può essere pubblicato su:
- **Netlify** – trascina la cartella `dist/` su [app.netlify.com](https://app.netlify.com)
- **Vercel** – `vercel deploy`
- **GitHub Pages** – con l'action Astro ufficiale
- **Hosting tradizionale** – carica il contenuto di `dist/` via FTP

---

## 🍷 Sezioni incluse
- ✅ Hero con immagine di sfondo e CTA
- ✅ Storia della cantina (Dal 1962)
- ✅ Menù dei vini (6 etichette DOC)
- ✅ Galleria fotografica
- ✅ Video YouTube integrato
- ✅ Contatti con mappa Google
- ✅ Pulsante WhatsApp
- ✅ Link Instagram e Facebook
- ✅ Design responsive mobile-first
- ✅ Animazioni scroll reveal
- ✅ SEO meta tags

---

*Progetto realizzato con ❤️ per la Cantina Ildavini – Abruzzo, Italia*
