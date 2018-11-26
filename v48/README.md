# Strängar

**Det första vi ska kolla på idag är hur man behandlar text som inte är syntax i Python.**<br>
All typ av text som inte är syntax kallas för strängar.<br>
En sträng inom programmering kännetecknas i de flesta fall av att det finns dubbelcitattecken i början och slutet av texten.<br>
Exempel:
```python

string = "Detta är en sträng sparad i en variabel"

print("Man kan även skriva ut strängar till konsolen")


```

Man kan även slå ihop strängar med en operation som kallas för konkatenering. 
Den använder samma tecken som addition, d.v.s. plustecknet. **MEN** försöker du att konkatenera nummer och strängar så kommer programmet inte att veta hur den ska tolka plustecknet och således att krascha. För att undvika detta så får vi använda oss utav tre inbyggda funkioner som gör om tal till strängar och vise versa.

* ```int()``` - Gör om sträng till heltal
* ```float()``` - Gör om sträng till decimaltal
* ```str()``` - Gör om alla typer av tal till sträng

Exempel:
```python

int_tal =  5
str_tal = "5"

float_decimal = 10.5
str_decimal = "10.5"

int_sum = int_tal + int(str_tal) 
int_str = str_tal + str(str_tal) 

float_sum = float_decimal + float(str_decimal) 
float_str = str_decimal + str(float_decimal) 

# Fundera: Vad tror du att följande prints skriver ut?
print(int_sum)
print(int_str)
print(float_sum)
print(float_str)

```

Med hjälp av dessa tre funktioner så hjälper vi programmet att veta exakt hur den ska tolka de olika operatorerna 
Enda problemet som kan uppstå nu är om det vi skriver innuti funktionerna inte är korrekt formatterat. <br>
Exempelvis att vi skickar med bokstäver till funktionen ```float()```, då kommer inte programmet veta hur den ska tolka 
bokstäver som tal och även då krascha. Lösningen på det problemet väntar vi lite med till senare här nere.

<hr>

# Input

**Majoriteten av alla program som skapas är beroende av någon sorts data eller interaktion.**

Och för att läsa av just input från konsolen in till en variabel i Python så använder vi oss utav funktionen ```input()```.<br>
Den fungerar som så att man innanför parenteserna kan (om man vill) skriva en text/fråga till användaren och sedan måste användaren skriva in något i konsolen.<br>
**Observera att om programmet inte får någon input från konsolen så kommer det att fastna på den raden.**

Ett simpelt program med input kan se ut så här:
```python
# Skapa variabel och vänta på input från användaren
name = input("Hej! Vad heter du? ")

# Skriv ut en hälsning
print("Välkommen " + name)
```

Detta program ber änvändaren skriva in sitt namn och skriver sedan ut en liten hälsning tillbaka. <br>
Denna typ av program fungerar jättebra med strängar, men så fort du vill läsa in tal kommer du märka att det blir problem.
Exempel:
```python
# Läs in och lagra input
tal1 = input("Skriv in två tal att multiplicera: ")
tal2 = input()

# Beräkna
produkt = tal1 * tal2

# Skriv ut resultat
print("Svar: " + produkt)
```
*Kan du gissa var det blir fel?*
<br><br><br>
Svar:<br>
Eftersom Python inte vet vad du skriver in i konsolen så kommer den **alltid** att behandla input som text, eller rättare sagt strängar.
Det gör att datorn i vårt fall inte vet hur den ska bete sig när vi vill multiplicera två strängar.
Lösningen på detta är att skriva antingen ```int()``` eller ```float``` runtom variablerna på den raden där vi multiplicerar dem. Sedan när vi ska skriva ut resultatet tillsammans med en annan sträng så blir det också fel. Då måste vi göra om det till en sträng igen med hjälp av ```str()```. Om vi skriver om koden så att det verkligen fungerar så ser det ut såhär:
```python
# Läs in och lagra input
tal1 = input("Skriv in två tal att multiplicera: ")
tal2 = input()

# Beräkna
produkt = int(tal1) * int(tal2)

# Skriv ut resultat
print("Svar: " + str(produkt))
```

<hr>

# Villkor
Genomgång



<hr>

# Avancerat
Om vi hinner

