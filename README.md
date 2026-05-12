# ZG Band — Sito Web

## Come mettere online il sito (GRATIS con GitHub Pages)

### Primo setup (una volta sola)
1. Vai su **github.com** e crea un account gratuito
2. Clicca il pulsante **"+"** in alto a destra → **"New repository"**
3. Nome del repository: `zgband` (o quello che preferisci)
4. Spunta **"Public"**
5. Clicca **"Create repository"**
6. Trascina TUTTI i file di questa cartella (index.html + cartella images) nella pagina
7. Clicca **"Commit changes"**
8. Vai in **Settings → Pages** (nel menu a sinistra)
9. Sotto "Source" scegli **"main"** e clicca **Save**
10. Dopo 1-2 minuti il sito sarà online a: `https://TUONOME.github.io/zgband/`

---

## Come modificare il sito

### Aggiungere un video YouTube
1. Vai su YouTube, apri il video
2. Clicca **"Condividi" → "Incorpora"**
3. Copia il codice che inizia con `<iframe...`
4. Apri `index.html` su GitHub (clicca il file → matita per modificare)
5. Cerca `<!-- SLOT VIDEO 1 -->` 
6. Sostituisci il blocco `<div class="video-slot">...</div>` con il codice iframe copiato
7. Clicca **"Commit changes"**

### Aggiungere una foto nella galleria
1. Carica la foto nella cartella `images` su GitHub
2. Apri `index.html` e cerca `<!-- Foto 1 -->` (o 2, 3...)
3. Sostituisci il blocco `<div class="gallery-slot">...</div>` con:
   ```html
   <img src="images/NOME-TUA-FOTO.jpg" alt="Descrizione" style="width:100%;height:100%;object-fit:cover;border-radius:8px;">
   ```
4. Clicca **"Commit changes"**

### Aggiungere un nuovo evento
1. Apri `index.html` su GitHub
2. Cerca il commento `<!-- Per aggiungere altri eventi -->`
3. Togli i `<!--` e `-->` attorno al blocco evento di esempio
4. Modifica DATA, NOME EVENTO, LUOGO e ORARIO
5. Carica la foto dell'evento nella cartella `images`
6. Clicca **"Commit changes"**

### Modificare testo, email o telefono
1. Apri `index.html` su GitHub (matita per modificare)
2. Cerca il testo da cambiare (usa Ctrl+F)
3. Modificalo
4. Clicca **"Commit changes"**

---

## Struttura dei file
```
zgband-site/
├── index.html          ← il sito (tutto in un file!)
└── images/
    ├── zg-band.jpg     ← foto principale della band
    └── sagra-anguilla.jpg ← locandina evento
```
