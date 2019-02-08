Dokumentation

Dokumenation för serverprojektet.

### Steg 1 - Konfigurera SD-kortet

Innan vi kan starta vår Raspberry Pi behöver vi installera ett operativsystem på det SD-kort som kommer få agera hårddisk.
Detta görs enklast med programmet Etcher från Balena via [dennna länk](https://www.balena.io/etcher/). Etcher fungerar på dem flesta plattformar.  Vi behöver även ladda ner filen som vi ska skriva till SD-kortet, i detta fall operativsystemet Raspbian, vilket hittas via [denna länk](https://www.raspberrypi.org/downloads/raspbian/).

Innan vi kan skriva Raspbian med Etcher behöver du även extrahera zip-filen du precis laddade ner för att få fram en **.img** fil. Öppna sedan Etcher och välj **.img** filen och vilken enhet du vill skriva till, och tryck sedan på knappen **Flash!**

När programmet har skrivit klart filen är du redo att sätta i kortet i din Raspberry Pi.

### Steg 2 - Anslut till SSH

För att ansluta till din Raspberry Pi via nätverket behöver vi ta reda på vilken IP-adress vår enhet har fått tilldelad av vår router.
Det går att göra på flera olika sätt, så välj ett av nedan alternativ:

- Ta reda på ip-adressen via din routers web-gränsnitt.
- Pinga **`raspberrypi.local`**
- Anslut till din raspberry pi med skärm och tangentbord och kör **ip** kommandot.

### Steg X - Uppdatera Raspbian

Kör nedan kommando för att uppdatera mjukvaran på din Raspberry Pi till senast tillgängliga. Bekräfta med Y eller N när du blir tillfrågad.

```bash
sudo apt update
sudo apt upgrade
```

### Steg X - Säkra upp din Raspberry Pi

Som standard får vi logga in med användaren **pi** med lösenordet **raspberrypi** över SSH och det är långt ifrån vad man skulle kalla säkert. Vi behöver därför skapa en ny användare, generera säkerhetsnycklar för SSH och sist men inte minst endast tillåta inloggningen över SSH med säkerhetsnycklar.















