# 📺 Lista IPTV + EPG con Proxy

Benvenuto nella tua **lista IPTV personalizzata** con **EPG** integrata e supporto proxy, perfetta per goderti i tuoi contenuti preferiti ovunque ti trovi!

---

## 🌟 Cosa include la lista?

- **🎥 Pluto TV Italia**  
  Il meglio della TV italiana con tutti i canali Pluto TV sempre disponibili.

- **⚽ Eventi Sportivi Live**  
  Segui in diretta **calcio**, **basket** e altri sport. Non perderti neanche un’azione!

- **📡 Sky e altro ancora**  
  Contenuti esclusivi: film, serie TV, sport e molto di più direttamente da Sky.

---

## 🔗 Link pronti all’uso

Queste liste utilizzano un proxy ospitato su **HuggingFace Spaces**.

- **Lista M3U**  
  [`https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/lista.m3u`](https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/lista.m3u)

- **EPG XML**  
  [`https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/epg.xml`](https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/epg.xml)

---

## 🧩 Proxy: come funziona

Se il proxy fornito non dovesse funzionare o preferisci crearne uno tuo, puoi farlo facilmente.

### ✅ Crea il tuo proxy personalizzato

- **Proxy base più stabile**:  
  [tvproxy (repo GitHub)](https://github.com/nzo66/tvproxy)

- **Proxy alternativo**:  
  [mediaflow-proxy](https://github.com/mhdzumair/mediaflow-proxy)

- **Per HuggingFace**  
  Usa questa repo ottimizzata: [hfmfp](https://github.com/nzo66/hfmfp)

---

## ⚙️ Personalizza il tuo proxy

### 1. Fai il fork della repo

Avvia creando un fork della repository proxy.

### 2. Modifica il file `.env` ed inserisci i tuoi dati.
Per includere **canali esteri**, utilizza il branch `world`.

---

> Se utilizzi **mediaflow-proxy**

> Ricorda di aggiornare anche il file `.github/workflows/main.yml` con `listaMFP.py` nella riga 27.

---

## 🚀 Esecuzione automatica con GitHub Actions

Dopo le modifiche:

1. Vai sulla sezione **Actions** della tua repo  
2. Avvia manualmente lo script  
3. Assicurati che **GitHub Actions sia abilitato** nella repository

---

## 🤝 Hai bisogno di aiuto?

Apri una **issue** o proponi un miglioramento con una **pull request**.  
Contribuire è sempre benvenuto!
