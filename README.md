# Cooking Class Arezzo — Ristorante Le Corniole

Sito web bilingue (EN/IT) per le cooking class del **Ristorante Le Corniole** di Arezzo, ottimizzato per Google (SEO) e per i motori di ricerca AI come ChatGPT, Perplexity e Claude (GEO).

## Struttura

| File | Descrizione |
|---|---|
| `index.html` | Homepage in **inglese** (la lingua di chi cerca "cooking class arezzo") |
| `it/index.html` | Versione **italiana** completa |
| `assets/css/style.css` | Stile del sito (palette toscana calda) |
| `assets/img/` | Foto generate con AI (scaricate dalla GitHub Action `fetch-images`) |
| `sitemap.xml` | Sitemap con alternates hreflang e immagini |
| `robots.txt` | Aperto a tutti i crawler, inclusi i bot AI |
| `llms.txt` | Scheda informativa per i motori AI (GEO) |

## Ottimizzazioni incluse

- **Dati strutturati JSON-LD**: `Restaurant` (LocalBusiness), `Product` con 3 offerte prezzo e recensioni, `FAQPage` → idonei ai rich results di Google (stelle, FAQ, prezzi).
- **hreflang EN/IT**, canonical, Open Graph, Twitter Card, meta geo (Arezzo, IT-AR).
- **Contenuto GEO-friendly**: fatti chiari e verificabili (prezzi, orari, indirizzo, cosa è incluso) + `llms.txt`.
- **Keyword target**: cooking class Arezzo, pasta making class Tuscany, corso di cucina Arezzo, tiramisù class, cooking class near Cortona.
- Recensioni reali dal PDF (USA, UK, Australia, Germania, Spagna, Paesi Bassi).
- Prenotazione a 1 tap: telefono, WhatsApp (pulsante flottante), email, mappa Google integrata.

## Come pubblicare (GitHub Pages)

1. Su GitHub: **Settings → Pages → Source: Deploy from a branch** → scegli questo branch, cartella `/ (root)`.
2. Il sito sarà su `https://radusbologa-ctrl.github.io/cooking-class-arezzo/`.

## Passi successivi consigliati (importanti per il posizionamento)

1. **Compra un dominio** tipo `cookingclassarezzo.it` o `cookingclassarezzo.com` e collegalo a GitHub Pages (Settings → Pages → Custom domain). Poi sostituisci `radusbologa-ctrl.github.io/cooking-class-arezzo` con il nuovo dominio in `index.html`, `it/index.html`, `sitemap.xml`, `robots.txt` e `llms.txt`.
2. **Google Business Profile**: crea/aggiorna la scheda "Ristorante Le Corniole" aggiungendo il servizio "Cooking Class" e il link al sito — è il fattore n.1 per le ricerche locali.
3. **Google Search Console**: verifica il sito e invia `sitemap.xml`.
4. **Recensioni**: chiedi agli ospiti di recensire su Google e TripAdvisor citando "cooking class" — poi aggiorna `reviewCount` nel JSON-LD di `index.html` con i numeri reali.
5. **GetYourGuide / Viator / Airbnb Experiences**: pubblica l'esperienza anche lì con link al sito (backlink + prenotazioni).
6. Verifica la **durata esatta della lezione** e aggiungila alle FAQ se vuoi (al momento non è indicata).

## Foto

Le foto sono generate con AI (Higgsfield). Quando avrai foto reali della cooking class, sostituisci i file in `assets/img/` mantenendo gli stessi nomi: le foto reali convertono meglio e Google le preferisce.
