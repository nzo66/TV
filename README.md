# 📺 Lista IPTV + EPG con Proxy

Benvenuto nel tuo setup personalizzabile di **lista IPTV** con **EPG**, supportata da un **proxy**

---

## 🔗 Lista gia' pronta

Queste liste utilizzano un proxy ospitato su HuggingFace Spaces.

- **Lista M3U**:  
  [`https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/lista.m3u`](https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/lista.m3u)

- **EPG XML**:  
  [`https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/epg.xml`](https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/epg.xml)

---

## 🧩 Funzionamento con Proxy

Se il proxy non funziona o vuoi avere il tuo, puoi:

### ✅ Creare il tuo proxy personalizzato:

🔗 Repo del proxy: [tvproxy](https://github.com/nzo66/tvproxy)

### Oppure:

🔁 Usa [mediaflow-proxy](https://github.com/mhdzumair/mediaflow-proxy)

---

## 🛠️ Come personalizzare il proxy

1. **Fai il Fork** di questa repository.

2. Modifica il file `lista.py`. Se vuoi includere anche **canali esteri**, usa il branch `world`.

---

### ✏️ Modifiche da effettuare:

#### 1️⃣ URL del Proxy

Sostituisci tutte le occorrenze di:

```
https://nzo66-piccolotest.hf.space
```

con **il tuo** URL HuggingFace, Render o self-hosted (es: `https://tuonome.hf.space`)

#### 2️⃣ Se usi [mediaflow-proxy](https://github.com/mhdzumair/mediaflow-proxy)

Modifica anche questo:

```diff
- /proxy/m3u?url=
+ /proxy/hls/manifest.m3u8?api_password=test123&d=
```

> 🔒 Ricorda di sostituire `test123` con la **tua password** del mediaflow-proxy.

📌 Il risultato sarà qualcosa del tipo:

```
https://tuoproxy.hf.space/proxy/hls/manifest.m3u8?api_password=miaPassword&d=
```

#### 3️⃣ URL dell’EPG

Cerca questo link (sempre nel file lista.py):

```
https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/epg.xml
```

E sostituisci:

```
nzo66/TV
```

con il tuo utente GitHub e il nome del fork (es. `tuonome/TV`).

---

## 🚀 Esecuzione con GitHub Actions

Una volta fatte le modifiche:

1. Vai su **Actions** nella tua repo
2. Avvia lo script manualmente
3. ✅ Assicurati di **abilitare i permessi di GitHub Actions** per questa repo

---

## 🤝 Supporto

Hai dubbi o vuoi contribuire? Apri una issue o una pull request!
