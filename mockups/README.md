# Mockup Prodotti — WonderSpit Product Designer

## Struttura cartelle

I file devono rispettare ESATTAMENTE questi nomi e percorsi.
Il designer li legge automaticamente da GitHub tramite URL.

```
mockups/
  tshirt/
    fronte.png
    retro.png
    manica_sx.png    ← opzionale, aggiungere quando disponibile
    manica_dx.png    ← opzionale, aggiungere quando disponibile

  felpa/
    fronte.png
    retro.png
    manica_sx.png    ← opzionale
    manica_dx.png    ← opzionale

  hoodie/
    fronte.png
    retro.png
    manica_sx.png    ← opzionale
    manica_dx.png    ← opzionale

  manica_lunga/
    fronte.png
    retro.png
    manica_sx.png    ← opzionale
    manica_dx.png    ← opzionale

  vneck/
    fronte.png
    retro.png
    manica_sx.png    ← opzionale
    manica_dx.png    ← opzionale
```

## Regole importanti

- Nomi file: MINUSCOLO, con underscore _ (no spazi, no maiuscole)
- Formato: PNG con sfondo TRASPARENTE (solo ombre/pieghe visibili)
- Dimensioni consigliate: 800x800px o superiore
- I tab "Sinistra" e "Destra" nel designer appaiono SOLO se il file esiste
- fronte.png e retro.png sono OBBLIGATORI per ogni prodotto

## URL base GitHub

I file vengono letti da:
https://raw.githubusercontent.com/Mondor89/Product-Designer/main/mockups/

Esempio URL completo:
https://raw.githubusercontent.com/Mondor89/Product-Designer/main/mockups/tshirt/fronte.png

## Stato attuale

| Prodotto     | Fronte | Retro | Manica Sx | Manica Dx |
|--------------|--------|-------|-----------|-----------|
| tshirt       | ✅     | ✅    | ❌        | ❌        |
| felpa        | ✅     | ✅    | ❌        | ❌        |
| hoodie       | ✅     | ✅    | ❌        | ❌        |
| manica_lunga | ✅     | ✅    | ❌        | ❌        |
| vneck        | ✅     | ✅    | ❌        | ❌        |
