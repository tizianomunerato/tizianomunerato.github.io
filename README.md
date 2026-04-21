# Fitness Dashboard PWA

Questa cartella contiene una Progressive Web App statica, installabile su telefono.

## Come provarla in locale

Serve un piccolo server HTTP locale. Due opzioni semplici:

### Python

```bash
cd fitness-pwa
python -m http.server 8000
```

Poi apri il browser su `http://localhost:8000`.

### Node.js

```bash
npx serve .
```

## Come installarla sul telefono

1. Pubblica questa cartella su un hosting HTTPS, oppure provala in locale.
2. Apri la pagina dal browser del telefono.
3. Usa “Aggiungi a schermata Home” oppure il prompt di installazione se compare.

## Cosa include

- piano data-driven in `index.html` dentro `PLAN_CONFIG`
- salvataggio locale con `localStorage`
- timer automatici e manuali
- service worker per uso offline base
- manifest PWA

## Limiti attuali del prototipo

- segnali audio semplici via Web Audio API
- nessuna sincronizzazione cloud
- nessuna vibrazione nativa dedicata
- configurazione ancora interna al file HTML, non in JSON esterno
