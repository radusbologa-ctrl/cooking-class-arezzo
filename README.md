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

1. Rendi il repository **pubblico** (Settings → General → Danger Zone → Change visibility) — richiesto per GitHub Pages gratuito.
2. Su GitHub: **Settings → Pages → Source: Deploy from a branch** → scegli questo branch, cartella `/ (root)`.
3. Sempre in **Settings → Pages → Custom domain**: inserisci `www.cookingclassarezzo.it` e, quando disponibile, spunta **Enforce HTTPS**.
4. Su **Register.it → Gestione DNS** del dominio `cookingclassarezzo.it` crea questi record:

   | Tipo | Host | Valore |
   |---|---|---|
   | A | `@` | `185.199.108.153` |
   | A | `@` | `185.199.109.153` |
   | A | `@` | `185.199.110.153` |
   | A | `@` | `185.199.111.153` |
   | CNAME | `www` | `radusbologa-ctrl.github.io` |

   (elimina eventuali record A o CNAME preesistenti su `@` e `www`, come la pagina parcheggio di Register)

5. Attendi la propagazione DNS (da pochi minuti a qualche ora). Il sito risponderà su `https://www.cookingclassarezzo.it/` e `cookingclassarezzo.it` reindirizzerà automaticamente.

## Passi successivi consigliati (importanti per il posizionamento)

1. **Google Business Profile**: crea/aggiorna la scheda "Ristorante Le Corniole" aggiungendo il servizio "Cooking Class" e il link al sito — è il fattore n.1 per le ricerche locali.
2. **Google Search Console**: verifica il sito e invia `sitemap.xml`.
3. **Recensioni**: chiedi agli ospiti di recensire su Google e TripAdvisor citando "cooking class" — poi aggiorna `reviewCount` nel JSON-LD di `index.html` con i numeri reali.
4. **GetYourGuide / Viator / Airbnb Experiences**: pubblica l'esperienza anche lì con link al sito (backlink + prenotazioni).
5. Verifica la **durata esatta della lezione** e aggiungila alle FAQ se vuoi (al momento non è indicata).

## Foto

Le foto `real-*.jpg` e `tuscany-landscape.jpg` sono foto reali della cooking class (da ilpoggiolinodoro.it); le altre sono generate con AI (Higgsfield). Quando avrai altre foto reali, sostituisci i file in `assets/img/` mantenendo gli stessi nomi: le foto reali convertono meglio e Google le preferisce.
