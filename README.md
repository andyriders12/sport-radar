# Sport Radar Android 1.0

Progetto Android WebView con HTML 13.5 integrato in `app/src/main/assets/index.html`. Il sito GitHub Pages continua a usare `index.html` nella radice.

## Da Samsung
1. Aprire repository `andyriders12/sport-radar`, ramo `main`.
2. Caricare i file e le cartelle del progetto preservando la struttura (non caricare solo lo ZIP come file). Il sito esistente `index.html` può rimanere invariato.
3. In `.github/workflows/` aggiungere `android-apk.yml` (non sostituire `main.yml`, che è un workflow di prova).
4. Aprire **Actions** > **Compila APK Sport Radar** > **Run workflow**.
5. Aprire la compilazione riuscita e scaricare **SportRadar-APK** da Artifacts; estrarre `app-debug.apk` e installarlo.

APK di debug firmato automaticamente per test; non è una release per Play Store. La compilazione è da verificare su GitHub. Internet necessario per dati meteo e spot. L'HTML è integrato, non caricato dal sito.
