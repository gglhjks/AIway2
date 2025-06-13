# 🌐 AIway

> “Impara, applica, crea: l’intelligenza artificiale al tuo servizio”

**AIway** è una piattaforma educativa e interattiva per imparare e applicare l'intelligenza artificiale nella scuola, nel lavoro, nella creatività e persino per guadagnare. È pensata per utenti di qualsiasi livello, anche principianti.

---

## ✨ Funzionalità principali

- 👤 Profilo utente locale
- 💬 Domande dirette all’IA (OpenAI API)
- 🧠 Quiz interattivo con punteggio salvato
- 📁 Storico personale e salvataggio locale
- 🔁 Esporta/Importa dati in JSON
- ⚙️ Impostazioni account
- 📱 Responsive e accessibile da tutti i dispositivi

---

## 🧰 Stack Tecnologico

- React + Vite
- Tailwind CSS
- LocalStorage
- OpenAI API (opzionale)

---

## 📦 Come installare il progetto

```bash
git clone https://github.com/TUO-USERNAME/aiway.git
cd aiway
npm install
npm run dev
```

---

## 🚀 Deploy su Vercel

1. Verifica che siano presenti i file:
   - `vite.config.js`
   - `vercel.json`
   - `package.json`
2. Pusha il progetto su GitHub
3. Vai su [https://vercel.com](https://vercel.com), clicca su **"Add New Project"**
4. Seleziona il repo `aiway`, framework: `Vite`
5. Clicca **Deploy**

---

## 🌐 Routing per SPA

File `vercel.json`:

```json
{
  "rewrites": [
    { "source": "/(.*)", "destination": "/index.html" }
  ]
}
```

File `vite.config.js`:

```js
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'

export default defineConfig({
  plugins: [react()],
  base: './',
  build: {
    outDir: 'dist'
  }
})
```

---

## 📄 Licenza

© 2025 AIway – Tutti i diritti riservati. Distribuito per fini educativi.

---

**Progetto creato con ❤️ per rendere l’intelligenza artificiale accessibile a tutti.**
