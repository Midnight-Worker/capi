# capi
## Capacitor with Ionic

# 1. Projekt anlegen
mkdir meine-app
cd meine-app
mkdir www

# 2. npm initialisieren
npm init -y

# 3. Capacitor installieren
npm install @capacitor/core@8 @capacitor/android@8
npm install -D @capacitor/cli@8

# 4. index.html in www/ erstellen
# Ionic über CDN einbinden

# 5. Capacitor initialisieren
npx cap init "Appname" "de.midnight.appid" --web-dir www

# 6. Android-Projekt erzeugen (nur einmal!)
npx cap add android

# 7. Webdateien nach Android kopieren
npx cap sync android

# 8. Android Studio öffnen
npx cap open android
