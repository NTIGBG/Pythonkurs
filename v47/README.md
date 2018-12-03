# Intro

**Välkommen** till denna introduktionskurs i programmering!<br>
Vi kommer i denna kurs att lära oss programmeringsspråket Python. <br>
Python är ett bra språk att lära sig om mam är helt ny till programmerint då Python har en *relativt enkel* syntax som framförallt inte skiljer sig så mycket ifrån hur vi människor skriver till vardags.<br><br>

**Syftet med kursen** är att främst matematiklärare ska lära sig om programmering på ett interaktivt sätt samt att enkelt och smidigt kunna föra det direkt vidare ut i sina klassrum. <br>
Under kursens gång kommer vi att lära oss många nya begrepp vilka är viktigare än man kan tro att hålla koll på.<br>
Därför så kommer det att till varje vecka att finnas en tillhörande ordlista längst ned med förklaringar till alla nya och svåra ord. 
<br><br>
**I denna övning** kommer vi att lära oss om den grundläggande syntaxen för programmering i just språket Python samt hur man skapar loopar och med hjälp av dessa enkelt kan beräkna olika matematiska summor. <br>
Men innan vi börjar koda så måste vi fixa lite saker först. Scrolla ner till nästa del och följ instruktionerna.
<hr>

# Komma igång

1. Börja med att registrera er på repl.it genom att klicka på denna [länk](https://repl.it/).<br>
   *Det är här vi kommer att koda och spara allting vi gör i kursen.*

2. När du registrerat dig kan du klicka på knappen till höger, "Start coding now".<br>
<img src="https://gyazo.com/2306e17c235b266ebdd1ea52260180ca.png" width="500" height="200" /><br>

3. Leta sedan på och välj sedan språket Python, som troligtvis står högst upp.<br>
<img src="https://gyazo.com/21bfbf4e50428892d4a733e2112baf99.png" width="500" height="200" /><br>

4. Nu borde du se denna vy, om allting gått rätt till.<br>
<img src="https://gyazo.com/28c773fd2e6999409f4ba4a88e09c045.png" width="800" height="300" /><br>

5. Snyggt! Nu kan vi börja programmera på riktigt!

<hr>

# Variabler

Det första vi ska kolla på är variabler. Variabler inom programmering används för att lagra värden. 
Inom alla programmeringsspråk så finns det olika regler för hur man tillåts namnge variabler.
I språket Python är reglerna som följer:
* Variabelnamn får **enbart innehålla** bokstäver, siffror och "_".
* Variabelnamn får **enbart börja** på en bokstav eller "_".

Här är exempel på variabelnamn som är giltiga respektive ogiltiga:<br>
* Giltiga variabelnamn:
```
tal1
tal_2
TAL3
_4
__Tal5
```
* Ogiltiga variabelnamn:
```
tal-1
tal.2
3tal
tal?
$tal5
```
*Man kan även använda åäö i sina variabelnamn, men det är inte att rekommendera då det ibland kan ställa till problem.*

**(!)** <br>
Viktigt att tänka på när vi börjar koda är att allting vi skriver är i Python case-sensetive, vilket innebär att språket är känsligt på om vi använder stora eller små bokstäver. <br>
Det innebär i praktiken att variablerna ```tal1``` och ```Tal1``` behandlas helt olika.
<br>


Syftet med variabler är, som tidigare nämnt, att ge dem olika värden och detta gör vi med tilldelningsoperatorn "=".<br>
Exempel:
```python
tal1 = 501
tal_2 = 26
TAL3 = 809
_4 = 50505
__Tal5 = 6
```
<br><br>

Att bara skapa variabler och ge dem värden är inte så värst givande och kanske inte så roligt heller för den delen.<br>
Men för att få lite feedback på det vi gör ska vi därför skriva ut värdena på våra variabler till konsolen.<br>
Det gör vi med en inbyggd funktion som heter ```print()```.<br>
Den används genom att skriva in namnet på den variabel vi vill skriva ut innanför de två parenteserna. Det kan se ut såhär:

```python
# Skapa variabel och tilldela värde
tal = 56

# Skriv ut till konsolen
print(tal)
```

Testa själv att kopiera in koden ovan till repl.it och klicka på run för att se vad som händer.<br>
<img src="https://gyazo.com/3daf509796f595bd2a38422aac7340ba.png" width="400" height="200" /><br>

<hr>

# Räkneoperatorer

För att kunna räkna så måste vi självklart använda oss utav räkneoperatorer eller aritmetiska operatorer. Men i Programmering så kan vi inte skriva som vi gör på papper med exempelvis exponenter lite ovanför siffror och bråkstreck ibland eller snestreck ibland. Vi kan bara använda oss utav vanliga tecken som finns på tangentbordet och skriva dem på en och samma rad och datorn måste ha tydliga regler för vad som betyder vad. Därför har man fått bestämma sig för hur man ska skrva olika räknesätt i kod och även vilka räknesätt man vill ha inbyggda i olika språk. Det kan variera mellan olika språk och i just språket Python finns det 7 st olika inbyggda räkneoperatorer som används vid grundläggande matematiska beräkningar.<br>
Dessa är som följer:

Operator | Räknesätt | Exempel | Värde
:---------:|:-----------:|:---------:|:-----:
\+ | addition| tal1 = 2 \+ 2 | 4
\- | subtraktion| tal2 = 5 \- 8 | -3
\* | multiplikation| tal3 = 2 \* 3 | 6
/ | division| tal4 = 15 / 2 | 7.5
% | modulus (rest)| tal5 = 8 % 3 |   2
\*\* | upphöjt till | tal6 = 2 \*\* 3  | 8
// | heltalsdivision | tal7 = 15 // 2 | 7

**Observera att heltalsdivision räknar ut kvoten och sedan avrundar nedåt till närmsta heltal.**

Här har jag förberett ett exempel med räkneoperatorer som ni kan kolla på och leka lite med: *Testa gärna att blanda olika räknesätt på samma rad* <br>
<iframe height="400px" width="100%" src="https://repl.it/@JoakimOhlsson/Rakneoperatorer?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

Om ni inte märkt det redan så håller Python koll på de olika prioriteringar som räknesätten har. Dvs:<br>
1. Parenteser
2. Potenser
3. Multiplikation,division
4. Addition,subtraktion

Datorn räknar alltid rätt och det är därför viktigt att du skriver exakt det du vill att datorn ska utföra. 
Man kan självklart applicera parenteser på olika räknesätt och variabler för att öka prioriteringen enligt ordningen ovan.

Testa nu själv att beräkna och skriva ut följande uttryck: <br>
<img src="https://gyazo.com/832acc0a085b31743eaab595b5c80d8b.png" width="150" height="100" /><br>

<hr>

# Loopar 

Loopar inom programmering är ungefär precis som det låter: någonting som går runt som en loop, eller mer korrekt: en kod som körs flera gånger.<br>
Man kan alltså med hjälp av loopar köra en bestämd sekvens av kod ett X antal gånger. Detta är väldigt fördelaktigt framförallt för att slippa skriva samma kod flera gånger men också för att beräkna 


## For-loopar

For-loopar används när man vill göra någonting ett känt antal gånger. Till exempel om man vill skriva ut alla tal från 1-10. Då vet vi att vi vill loopa 10 gånger, så då använder vi en for-loop.

En for-loop i Python kan se ut såhär:
```python
for i in range (0,10):
  print("hej")
```
Denna loop kommer att skriva ut hej till konsolen 10 gånger.<br><br>

En loop i python beror alltid på en variabel och i exemplet ovan valde jag att kalla den för i.<br>
Variabeln i kommer att variera mellan talen \[0,10). Alltså kommer i att få värdena 0 till och med 9. (Men det blir 10 unika värden eftersom vi börjar på 0).
<br>
Här är en for-loop skriven med variabler som förklarar lite hur allt händer ihop:

```python
firstNumber = 0
lastNumber = 10
for variable in range (firstNumber, lastNumber+1):
  print(variable)
```
Det är viktigt med indenteringen av koden i samband med en loop. Det är nämligen den som bestämmer vilka rader kod det är som vi vill köra flera gånger. Så fort att vi tar tillbaka indenteringen så betyder det att koden innuti loppen är slut.


## Andra typer av loopar

Det är bra att veta om att det finns andra typer av loopar, men dessa kommer vi inte gå in på just nu.
