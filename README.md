# scarica-foto.py

✅ Contenuto incluso:

    README.md — guida all'uso con immagini e badge

    wiki/INSTALL.md — guida passo-passo per l’installazione

    .gitignore — per non caricare i token e credenziali

    Extra: esempio struttura cartelle

    google-photos-downloader/
├── scarica-foto.py

├── credentials.json       # NON pushare mai

├── README.md

├── wiki/

│   └── INSTALL.md

├── .gitignore

# 📸 Google Photos Downloader (multi-account, con ripresa automatica)

Uno script Python per scaricare tutte le tue foto da Google Foto, supporta:

- ✅ Autenticazione con account Google
- ✅ Supporto multi-account
- ✅ Scaricamento in blocchi (con ripresa)
- ✅ Auto-refresh del token
- ✅ Salvataggio avanzamento per sessioni multiple

> Creato per funzionare facilmente su Linux Mint, openSUSE e altre distro Linux.

---

## 🚀 Avvio rapido

```bash
git clone https://github.com/tuo-username/google-photos-downloader.git
cd google-photos-downloader
pip install -r requirements.txt
python3 scarica-foto.py
📦 Requisiti

    Python 3.11+

    File credentials.json scaricato da Google Cloud Console (vedi wiki/INSTALL.md)




=== GESTIONE MULTI-ACCOUNT GOOGLE FOTO ===
Account disponibili:
 1) mario@gmail.com
 2) ➕ Usa un nuovo account Google
2. 🔑 Crea credenziali su Google Cloud Console

    Vai su Google Cloud Console

    Crea un progetto nuovo

    Vai su API e servizi > Libreria e attiva:

        ✅ Google Photos Library API

    Vai su API e servizi > Credenziali

        Crea credenziali OAuth client ID

        Tipo: App desktop

    Scarica il file credentials.json

    Copialo nella stessa cartella dello script

3. ▶️ Avvia lo script

python3 scarica-foto.py

Ti chiederà:

    di scegliere un account (se già presente)

    o di autenticarti con uno nuovo (si aprirà il browser)

4. 💾 Dove vengono salvati i file?

    I token di accesso: tokens/token_<email>.json

    Lo stato dei download: downloads/downloaded_ids_<email>.json

    Le foto: nella cartella scelta al momento del download

5. 📋 Consigli

    NON committare il file credentials.json o i token

    Usa .gitignore per evitarlo (già incluso)

    Puoi usare lo script per più account Google senza problemi

6. 🐧 Testato su

    Linux Mint 21

    openSUSE Leap 15.5


---

### 📄 `.gitignore`

```gitignore
# Non condividere file sensibili
credentials.json
tokens/
downloads/
__pycache__/
*.pyc
