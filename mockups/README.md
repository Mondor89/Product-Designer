# Mockup Prodotti — WonderSpit Product Designer

## Come funziona il cambio colore

Il designer colora la t-shirt cambiando i pixel del PNG direttamente nel browser.
Per farlo bene, il PNG deve rispettare queste regole:

- **Sfondo trasparente** — fuori dalla sagoma del prodotto non ci deve essere nulla
- **Prodotto bianco o grigio chiaro** — il colore scelto dall'utente sostituisce il bianco mantenendo le ombre e le pieghe visibili
- Se il prodotto è colorato nel PNG (es. rosso) → la colorazione non funziona bene
- Se lo sfondo non è trasparente → lo sfondo si colora invece della t-shirt

---

## Come preparare un mockup

### Strumento consigliato: Canva Pro

1. Trova o crea l'immagine della t-shirt (bianca, su sfondo bianco)
2. In Canva: **Modifica foto → Rimuovi sfondo** (rimuove automaticamente lo sfondo)
3. Scarica: **Condividi → Scarica → PNG → spunta "Sfondo trasparente"**
4. Controlla che il file scaricato sia trasparente (vedi sezione sotto)

### Alternativa gratuita: remove.bg

1. Vai su [remove.bg](https://www.remove.bg/it)
2. Carica il PNG della t-shirt (sfondo bianco va benissimo)
3. Scarica il risultato — è già PNG trasparente

---

## Come controllare che il PNG sia trasparente

**Su desktop (Windows):**
- Apri il PNG con il visualizzatore foto di Windows
- Se lo sfondo è a scacchi grigi e bianchi → trasparente ✅
- Se lo sfondo è bianco → NON trasparente ❌

**Su desktop (Mac):**
- Apri con Anteprima
- Sfondo a scacchi = trasparente ✅

**Su mobile:**
- Non si vede la trasparenza — controllare sempre da PC prima di caricare

---

## Specifiche tecniche file

| Campo | Valore |
|-------|--------|
| Formato | PNG (obbligatorio) |
| Sfondo | Trasparente (RGBA) |
| Colore prodotto | Bianco o grigio chiaro |
| Dimensioni tshirt / felpa / vneck / manica_lunga | 530×630px |
| Dimensioni hoodie | 670×893px |
| Nome file | minuscolo, underscore (es. `fronte.png`) |

---

## Struttura cartelle

I nomi devono essere ESATTAMENTE questi — il designer li legge in automatico.

```
mockups/
  tshirt/
    fronte.png       ← obbligatorio
    retro.png        ← obbligatorio
    manica_sx.png    ← opzionale
    manica_dx.png    ← opzionale

  felpa/
    fronte.png
    retro.png
    manica_sx.png
    manica_dx.png

  hoodie/
    fronte.png
    retro.png
    manica_sx.png
    manica_dx.png

  manica_lunga/
    fronte.png
    retro.png
    manica_sx.png
    manica_dx.png

  vneck/
    fronte.png
    retro.png
    manica_sx.png
    manica_dx.png
```

---

## Come aggiungere un nuovo prodotto

1. Crea una cartella con il nome del prodotto (minuscolo, underscore)
2. Metti dentro `fronte.png` e `retro.png` trasparenti
3. Aggiungi il prodotto nel codice `index.html` nella sezione `PRODUCTS` (chiedi a Claude)
4. Carica tutto su GitHub — Netlify si aggiorna automaticamente

---

## Come sostituire un mockup esistente

1. Prepara il nuovo PNG (trasparente, dimensioni corrette)
2. Rinominalo esattamente come il vecchio (es. `fronte.png`)
3. Caricalo su GitHub nella stessa cartella — sovrascrive il vecchio
4. Netlify si aggiorna in circa 1 minuto

---

## Stato attuale mockup

| Prodotto | Fronte | Retro | Manica Sx | Manica Dx |
|----------|--------|-------|-----------|-----------|
| tshirt | ✅ | ✅ | ❌ | ❌ |
| felpa | ⏳ da fare | ⏳ da fare | ❌ | ❌ |
| hoodie | ⏳ da fare | ⏳ da fare | ❌ | ❌ |
| manica_lunga | ⏳ da fare | ⏳ da fare | ❌ | ❌ |
| vneck | ⏳ da fare | ⏳ da fare | ❌ | ❌ |

✅ = trasparente e funzionante
⏳ = da rifare con sfondo trasparente
❌ = non ancora creato
