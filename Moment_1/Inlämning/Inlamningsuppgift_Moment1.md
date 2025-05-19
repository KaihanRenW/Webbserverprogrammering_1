## Inlämningsuppgift – Moment 1: Lösningar, språk & webbserver-grund

### Syfte
Att visa att du kan:
1. Installera och köra Apache + PHP i XAMPP på Windows.  
2. Använda grundläggande PHP-kod för request/response och sessionshantering.  
3. Förstå och förklara skillnaden mellan statiskt och dynamiskt innehåll.  
4. Reflektera över HTTP-metodernas användning och säkerhetsaspekter.

### Uppgiftsbeskrivning
1. **Installation & test**  
   - Installera XAMPP enligt studieguiden och starta Apache.  
   - Ta en skärmdump av XAMPP Control Panel med Apache-grön “Running”.

2. **”Hello från XAMPP”-sida**  
   - Skapa `hello.php` i `C:\xampp\htdocs\` som skriver ut “Hello från XAMPP! Server-tid: <datum-tid>”.  
   - Besvara: Varför är det viktigt att server-tiden stämmer?

3. **Request-läsning**  
   - Skapa `request.php` som läser `$_SERVER['REQUEST_METHOD']`, `REQUEST_URI` och query-parametrar (se exempel i studieguiden).  
   - Besvara i en kort textfil:  
     - Vilken metod (GET/POST) bör användas när man ändrar data i en databas, och varför?

4. **Sessionsräknare**  
   - Skapa `visits.php` som använder `session_start()` för att räkna hur många gånger just du har besökt denna sida.  
   - Förklara kort: Varför används sessioner istället för cookies för att räkna besök?

5. **Statisk vs Dynamisk**  
   - Skriv en kort jämförelse (max 200 ord) av för- och nackdelar med statiska respektive dynamiska webbplatser.  
   - Ge ett konkret exempel (t.ex. portfolio vs webbshop).

### Inlämningsformat
Samla allt i en mapp, pusha till github:

- **Kodfiler**:
  - `hello.php`
  - `request.php`
  - `visits.php`
- **Dokument** (Markdown):
  - Skärmdumpar (Installation)
  - Svar på reflektionsfrågor (punkter 2, 3 och 4)
  - För- och nackdelsjämförelse (punkt 5)

### Bedömningskriterier
| Delmoment           | Godkänt (G)                                                       | Väl Godkänt (VG)                                                  |
|---------------------|-------------------------------------------------------------------|-------------------------------------------------------------------|
| Installation & test | XAMPP är installerat, Apache körs (skärmdump).                    | Korrekt tidszon, inga fel i loggar.                               |
| Hello-sida          | Visar korrekt meddelande och tid.                                 | Egen funktion för formatering av datum/tid.                       |
| Request-läsning     | Läser metod, URI och query; korrekt förklarat GET vs POST.        | Gör enkel POST-hantering också, motiverar med RFC-argument.        |
| Sessions-räknare    | Rätt session-räkning och grundläggande förklaring.                | Hantering av session timeout, förklaring av säkerhetsaspekter.    |
| Statisk vs Dynamisk | Kort jämförelse med tydliga för- och nackdelar.                   | Tar upp caching-strategier och hybridlösningar.                   |

