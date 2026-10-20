# 13 månader – mobil kalenderprototyp

## Kalenderregler
- År 0 börjar den 21 december 98 e.Kr.
- Varje nytt kalenderår börjar alltid den 21 december.
- 13 månader med 28 dagar vardera (364 dagar).
- Efter månaderna följer en fristående nyårsdag. En andra fristående dag läggs till när kalenderåret innehåller den gregorianska 29 februari.
- Eftersom kalenderåret går från 21 december till 20 december, avgörs den extra dagen av om den gregorianska februari som ligger inne i just det intervallet har 29 dagar.
- Måndag är första veckodagen i varje månad; veckodagarna upprepas likadant i alla månader och pausas under nyårsdagarna.
- Händelser sparas med sitt vanliga gregorianska datum.

## Starta
Öppna `index.html` i en webbläsare för att prova appen. För installation som PWA/offline-app krävs att filerna publiceras på en HTTPS-webbserver (eller körs via localhost); öppna sedan sidan i Chrome på Android och välj **Installera app** / **Lägg till på startskärmen**.

## Kalenderkoppling
- **Exportera .ics** skapar en kalenderfil som kan importeras i Google Kalender, Outlook och andra appar.
- **Säkerhetskopiera** exporterar appens lokala händelser som JSON.
- **Återställ backup** importerar JSON.
- Automatisk tvåvägssynkronisering är inte implementerad. För det behövs OAuth/Google Calendar API eller en serverlösning, inklusive appens klient-ID och användarens uttryckliga godkännande.

## Viktigt
Händelser lagras i webbläsarens lokala lagring på den här enheten. Rensa inte webbplatsdata utan att först exportera en backup.


## Installera på Android
Ladda upp `manifest.json`, `sw.js`, `icon-192.png` och `icon-512.png` i samma mapp som `index.html` på GitHub Pages. De aktiverar installationsmetadata och grundläggande offline-cache.
