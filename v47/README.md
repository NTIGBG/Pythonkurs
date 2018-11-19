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
<img src="https://gyazo.com/28c773fd2e6999409f4ba4a88e09c045.png" width="800" height="400" /><br>

5. Bra! Nu kan vi börja programmera på riktigt!

<hr>

# Python - Variabler

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

<hr>

# Räkneoperatorer

