# PREREQUISITI

✅ Cosa ti serve:
 - Un account Google.
 - Un progetto su Google Cloud Console. https://console.cloud.google.com
 - Abilitare Photos Library API.
 - Scaricare il file credentials.json per OAuth.
 - Installare le librerie Python necessarie.

🔧 Step-by-step Setup
1. Crea un progetto e abilita l'API:

    Vai su console.cloud.google.com.

    Crea un nuovo progetto.

    Vai su “API e servizi” → “Libreria” → cerca e abilita Google Photos Library API.

    Poi vai su “Credenziali” → “Crea credenziali” → OAuth Client ID.

    Tipo applicazione: Desktop.

    Scarica il file credentials.json.

    Inserisci il file credentials.json nella directory dov'è presente il file `scarica-foto.py`

## 1. 🔧 Installa Python e le dipendenze

Assicurati di avere Python 3.11+ installato:

```bash
python3 --version
```

## Poi installa i pacchetti necessari:

``` pip install -r requirements.txt ```

Oppure manualmente:

``` pip install google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client tqdm requests ```
