# Diario di un fumatore, versione web installabile

Questo pacchetto trasforma Diario di un fumatore in un'app web che chiunque può aggiungere alla schermata Home di iPhone e Android con un semplice link. Non servono Mac, iPhone né App Store. Tempo necessario: circa 15 minuti. Tutto è gratuito.

## Pubblicare l'app su GitHub Pages

1. **Decomprimi il pacchetto.** Estrai `MenoFumoWeb.zip`. Dentro trovi `index.html`, `sw.js`, `manifest.webmanifest` e le cartelle `icons` e `fonts`.
2. **Crea un account GitHub.** Vai su **github.com**, scegli Sign up e conferma l'email. Scegli un nome utente semplice: farà parte dell'indirizzo dell'app.
3. **Crea un repository.** In alto a destra premi **+** e poi **New repository**. Come nome scrivi `diario-di-un-fumatore`. Lascia selezionato **Public** e premi Create repository.
4. **Carica i file.** Nella pagina del repository premi il pulsante **Add file**, in alto a destra sopra l'elenco dei file, e scegli **Upload files**. Se il repository è ancora vuoto trovi anche il link **uploading an existing file**: è la stessa cosa. Trascina tutti i file e le due cartelle che hai estratto. Le cartelle si possono trascinare solo da un computer. Non trascinare il file zip e nemmeno la cartella che li contiene. Aspetta la fine del caricamento e premi **Commit changes**. Poi controlla che `index.html` compaia subito nell'elenco del repository, non dentro un'altra cartella.
5. **Attiva GitHub Pages.** Vai in **Settings**, poi **Pages**. In Build and deployment scegli Source: **Deploy from a branch**. Come Branch scegli `main` e come cartella `/ (root)`. Premi Save.
6. **Aspetta e apri il link.** Dopo uno o due minuti, in cima alla stessa pagina compare l'indirizzo `https://TUONOME.github.io/diario-di-un-fumatore/`. Aprilo: deve comparire l'app. Se vedi un errore 404, aspetta ancora un minuto e ricarica.
7. **Condividi il link.** Manda l'indirizzo alle persone, insieme alle istruzioni qui sotto per aggiungere l'app alla schermata Home.

Alla fine, nel repository i file devono essere organizzati così:

```
diario-di-un-fumatore/
  index.html
  sw.js
  manifest.webmanifest
  icons/
  fonts/
```

## Come la installano le altre persone

- **iPhone.** Apri il link in **Safari**. Tocca il tasto Condividi (il quadrato con la freccia), poi **Aggiungi a Home** e **Aggiungi**. Da quel momento usa sempre l'icona sulla Home.
- **Android.** Apri il link in **Chrome**. Tocca il menu con i tre puntini e poi **Installa app** (oppure Aggiungi a schermata Home).

## Aggiornare l'app

Per cambiare qualcosa, chiedimi la modifica e ti do i file nuovi. Nel repository premi **Add file**, poi **Upload files**, e carica i file nuovi: sostituiscono quelli vecchi. Apri `sw.js` e aumenta il numero nella riga `CACHE` (per esempio da v4 a v5), così i telefoni scaricano la novità. Chi ha l'app la vede alla riapertura, a volte dopo averla chiusa e riaperta due volte.

## Da sapere

- I dati restano sul telefono di ciascuno. Non c'è registrazione né server: nessuno, nemmeno tu, può vedere i dati degli altri.
- Dopo la prima apertura l'app funziona anche senza connessione.
- Safari e l'icona sulla Home hanno archivi separati. I dati inseriti in Safari prima di aggiungere l'icona non compaiono nell'app. Conviene aggiungere subito l'icona e usare solo quella.
- Cancellare l'icona cancella i dati. Per fare una copia: Impostazioni, poi Backup, poi Scarica il file di backup, e conservalo dove vuoi (anche nel tuo cloud personale). Da lì puoi anche ripristinarlo.
- I dati non si sincronizzano tra telefoni diversi o tra telefono e computer.
- Il repository pubblico contiene solo il codice dell'app, nessun dato personale.
