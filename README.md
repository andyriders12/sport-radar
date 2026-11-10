# Sport Radar — Android (versione di prova)

Questa app incorpora **Sport Radar 13.5**, con Snowboard, MTB, Wind Sport e Climbing. Non include Trekking.

## Compilare da Samsung, senza PC

1. Apri GitHub dal browser Samsung e crea un **nuovo repository vuoto** (ad esempio `sport-radar-android`).
2. Carica **tutti i file e le cartelle di questo ZIP**, mantenendo la struttura, nella radice del repository. **Non caricare il solo ZIP**: GitHub Actions deve vedere `.github/workflows/android-apk.yml` e `app/`.
3. Apri la scheda **Actions** del repository. Se richiesto, abilita i workflow.
4. Seleziona **Crea APK Sport Radar**, poi **Run workflow** (oppure attendi la compilazione automatica dopo il caricamento su `main`).
5. Attendi il segno di spunta verde; apri il job completato e scarica l'artifact **SportRadar-Android-APK**.
6. Estrai lo ZIP scaricato: al suo interno trovi **app-debug.apk**. Aprilo sul Samsung e autorizza l'installazione da questa fonte, se Android lo richiede.

## Note importanti

- È un **APK debug di prova**, non firmato per distribuzione Play Store. Per aggiornamenti stabili e pubblicazione servirà una firma release gestita in sicurezza.
- Le funzioni meteo, ricerche e link richiedono Internet. L'HTML è incluso nell'app.
- L'uso di WebView può avere differenze rispetto al browser Samsung: testare le quattro sezioni, i preferiti e i collegamenti esterni.
- Per cambiare la versione web, sostituisci `app/src/main/assets/index.html` con il nuovo HTML e ricompila.
- Non pubblicare password, chiavi API o file di firma nel repository.
