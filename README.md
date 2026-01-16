# 🌀 Tempest Store - Sito E-commerce TCG

Sito web per Tempest Store Ardea - Negozio di carte collezionabili TCG.

## 🚀 Come pubblicare su Vercel

### Metodo 1: Deploy diretto (più veloce)
1. Vai su [vercel.com](https://vercel.com) e accedi con GitHub
2. Clicca "Add New Project"
3. Seleziona "Import Git Repository" 
4. Scegli questa repository
5. Clicca "Deploy"
6. Il sito sarà online in ~1 minuto!

### Metodo 2: Da GitHub
1. Carica questi file su una nuova repo GitHub
2. Vai su Vercel → New Project → Import da GitHub
3. Deploy automatico

## 📝 Come modificare i prodotti

Apri `index.html` e cerca la sezione `const products = [...]` (circa riga 580).

Ogni prodotto ha questa struttura:
```javascript
{
    id: 1,                          // Numero univoco
    name: "Nome Prodotto",          // Nome visualizzato
    category: "pokemon",            // Categoria (pokemon, yugioh, onepiece, dragonball, accessori)
    price: 49.99,                   // Prezzo in EUR
    oldPrice: 59.99,                // Prezzo barrato (opzionale)
    image: "URL_IMMAGINE",          // Link immagine prodotto
    description: "Descrizione",     // Breve descrizione
    badge: "Novità",                // Etichetta (opzionale): "Novità", "Rara", "-15%", "Preordine"
    inStock: true                   // true = disponibile, false = esaurito
}
```

## 💳 Configurare PayPal REALE

1. Vai su [developer.paypal.com](https://developer.paypal.com)
2. Crea un'app e ottieni il Client ID
3. In `index.html`, cerca questa riga:
   ```html
   <script src="https://www.paypal.com/sdk/js?client-id=test&currency=EUR&locale=it_IT"></script>
   ```
4. Sostituisci `test` con il tuo vero Client ID

## 📱 Contatti configurati

- **WhatsApp**: 348 878 5584
- **Instagram**: @tempest_store_ardea_tcg
- **Facebook**: Tempest Store Ardea
- **Indirizzo**: Via Verona 1, 00040 Ardea (RM)

## 🎨 Personalizzazioni

### Cambiare colori
I colori sono definiti nelle variabili CSS all'inizio del file:
```css
:root {
    --slime-dark: #2d5a7b;
    --slime-mid: #4a8fb8;
    --slime-light: #7ec8e3;
    /* ... altri colori */
}
```

### Cambiare orari
Cerca "Orari" nel file e modifica:
```html
<p>Lun-Sab: 10:00 - 20:00<br>Dom: 15:00 - 20:00</p>
```

## 📂 Struttura file

```
tempest-store/
├── index.html      # Sito completo (HTML + CSS + JS)
├── logo.png        # Logo Tempest Store
├── package.json    # Configurazione progetto
└── README.md       # Questo file
```

## ✨ Funzionalità

- ✅ Catalogo prodotti con filtri per categoria
- ✅ Carrello con quantità modificabili
- ✅ Checkout PayPal integrato
- ✅ Ordine via WhatsApp con messaggio precompilato
- ✅ Design responsive (mobile-friendly)
- ✅ Animazioni e effetti visivi
- ✅ Mappa Google con indirizzo
- ✅ Link social media

## 🔧 Supporto

Per modifiche o assistenza, contatta chi ha creato il sito!

---
Made with 💙 for Tempest Store Ardea
