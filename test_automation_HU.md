# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

#### ✅ Mi a tesztelés célja? Mi nem az?
A tesztelés célja a szoftver hibáinak felfedezése és a rendszer funkcionalitásának biztosítása, hogy az megfeleljen a specifikációknak.

#### ✅ Mik a tesztelési alapelvek?
1.	A tesztelés nem teljeskörű.
2.	A hibák összetettsége növeli az erőfeszítéseket.
3.	A tesztelés hibákat talál, de nem oldja meg őket.
4.	A tesztelési költségek a fejlesztési fázissal nőnek.

#### ✅ Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?
Az egységtesztelés a kód legkisebb részeinek tesztelése. Fejlesztők felelősek érte.

#### ✅ Mik a tesztszintek, és mi a különbség köztük?
•	Egységteszt: Egyes kód részek tesztelése.
•	Integrációs teszt: Modulok közötti interakciók tesztelése.
•	Rendszerteszt: Az egész rendszer tesztelése.
•	Elfogadási teszt: Felhasználói tesztelés a rendszer megfelelőségéről.

#### ✅ Mi a különbség a verifikáció és a validáció között?
•	Verifikáció: A rendszer a megfelelő módon van építve.
•	Validáció: A rendszer megfelel a felhasználói igényeknek.

#### ✅ Mik a tesztelési típusok, és mi a különbség köztük?
•	Funkcionális: A szoftver funkcionalitásának tesztelése.
•	Nem funkcionális: Teljesítmény, biztonság tesztelése.

#### ✅ Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?
•	Fehér doboz: A kód teljes ismerete.
•	Szürke doboz: Részleges kódismeret.
•	Fekete doboz: Nincs kódinformáció, csak a bemenet és kimenet vizsgálata.

#### ✅ Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?
•	UAT: Felhasználók tesztelik a szoftvert.
•	Rendszerteszt: Fejlesztők tesztelik az egész rendszert.

#### ✅ Sorolj fel különbségeket a regressziós tesztelés, a füsttesztelés és az újratesztelés között!
•	Regressziós: A rendszer működése nem változott a módosítások után.
•	Füstteszt: Alapfunkciók gyors ellenőrzése.
•	Újratesztelés: Hibák után a javított funkciók tesztelése.

#### ✅ Mi a különbség a statikus és dinamikus tesztelés között?
•	Statikus: Kódvizsgálat futtatás nélkül.
•	Dinamikus: Kód futtatása közben végzett tesztelés.

### ✅ Hasonlítsd össze a V-modellt, a vízesés modellt és az Agile megközelítést a tesztelés szempontjából!
•	V-modell: Fejlesztés és tesztelés párhuzamosan történik.
•	Vízesés modell: Lineáris, szekvenciális folyamat.
•	Agile: Iteratív, rugalmas tesztelés a fejlesztés során.


<img src="https://t4.ftcdn.net/jpg/03/90/15/65/360_F_390156585_8w1lsOyICIAOvDCU8tExXW2QwLCOFwXD.jpg" alt="image" width="550" height="400">


<img src="https://i.imgur.com/S38EBJw.png" alt="image" width="550" height="400">   <img src="https://segedletek.level14.hu/assets/img/modszertan-vizeses.svg" alt="image" width="550" height="400">


<img src="https://promanconsulting.hu/wp-content/uploads/2022/03/agilis-modszertanok-optimized.jpg" width="550" height="400">





## Reporting, Bugs
<img src="https://moolya.com/blog/wp-content/uploads/2023/05/Bug-Report.png" alt="image" width="300" height="220">

#### ✅ Milyen lépéseket követnél egy hiba megtalálásakor?
Reprodukálás – újra lefuttatom az esetet, hogy biztos legyen a hiba.

Dokumentálás – képernyőképek, logok, környezet rögzítése.

Prioritás meghatározása – üzleti hatás és technikai súlyosság alapján.

Jelentés – hibajelentés készítése, rendszerbe rögzítés (pl. Jira).

#### ✅ Beszélj a gyakori tesztjelentésekről és részleteikről!
Pass/Fail riportok – tesztesetek eredményei.

Bug summary – hány hibát találtak, státuszuk.

Coverage riport – mennyi kódot fed le a tesztelés.

Trend riport – hibák alakulása az idő során.


#### ✅ Mit tartalmaz egy hibajelentés?
Összefoglaló – rövid, de pontos cím.

Lépések a reprodukáláshoz

Várt vs. tényleges eredmény

Környezet (verzió, böngésző, OS stb.)

Logok, képernyőképek, videók (ha szükséges)
#### ✅ Hogyan rangsorolnál egy hibát?
Súlyosság (Severity): technikai hatás – pl. crash vs. UI hiba.

Prioritás (Priority): üzleti fontosság – mikor kell javítani.

Felhasználói hatás + előfordulási gyakoriság alapján.

## Test Automation, Selenium
<img src="https://media.licdn.com/dms/image/C4D12AQE3GOyVsZazOw/article-cover_image-shrink_600_2000/0/1583830696602?e=2147483647&v=beta&t=bYHbKyhMoWsMgtEug6eSf3m0db5ZtGEl437TeS1qkfI" alt="image" width="320" height="220">

#### ✅ Melyik teszteseteket érdemes automatizálni és melyiket nem?
Ismétlődő regressziós tesztek

Stabil, ritkán változó funkciók

Nagy adathalmazon végzett tesztek (adatvezérelt)

Több böngészőn/konfiguráción futó tesztek (cross-browser)

Smoke és sanity tesztek


Egy alkalommal futtatott tesztek

Gyakran változó UI elemek

Tesztek, amelyeknél emberi megítélés kell (pl. dizájn, UX)

Exploratory vagy ad-hoc tesztelés

#### ✅ Írj le egy jó automatizált tesztet!
Stabil elem-azonosítás (ID-k)

Explicit várakozás

Egyértelmű ellenőrzés

Átlátható és újrafelhasználható
#### ✅ Mi a Selenium, Selenium IDE és Selenium WebDriver?
Selenium: Nyílt forráskódú tesztautomatizálási eszközkészlet webes alkalmazásokhoz.

Selenium IDE: Böngészőbe épülő kiegészítő (Chrome/Firefox), amely lehetővé teszi felvételek és lejátszások készítését – nem kódolóknak ideális.

Selenium WebDriver: Programozható API több nyelven (pl. Python, Java), amely lehetővé teszi komplex, rugalmas tesztek írását.

#### ✅ Hogyan lehet azonosítani a webes elemeket?
Azonosítási módok:

ID – ha egyedi, a legjobb választás.

Name – alternatív ID hiányában.

Class name – ha biztosan egyedi vagy jól strukturált.

Tag name – ritkábban, általában listák esetén.

XPath – rugalmas, de lehet törékeny.

CSS selector – gyorsabb, modernebb XPath alternatíva.


#### ✅ Hogyan lehet várni az elemekre, és mi lehet a probléma? Gyűjtsd össze a lehetséges hibákat és okokat!
Várakozás típusai:

time.sleep() – kerülendő, mert fix és lassít.

Implicit wait – globális várakozási idő.

Explicit wait – célzott várakozás adott feltételre (WebDriverWait + EC).

Gyakori hibák:

ElementNotInteractableException – elem létezik, de nem kattintható (pl. rejtett).

NoSuchElementException – nem található (rossz selector vagy még nem töltődött be).

TimeoutException – nem jelent meg időben az elem.
#### ✅ Hasonlítsd össze a POM és a Keyword Driven Testing megközelítéseket!
POM (Page Object Model):

Kódalapú, minden oldalnak saját osztálya van

Strukturált, jól karbantartható

Fejlesztői tudás szükséges

Keyword Driven Testing:

Kulcsszavakkal írható teszt (pl. „Click”, „Input”)

Kevesebb programozás, manuális tesztelők is használhatják

Lassabb karbantartás, de gyors kezdés

#### ✅ Mi a különbség a TDD és BDD között?
TDD (Test Driven Development):

Kód előtt írunk egységtesztet

Fejlesztőknek szól

Technikai nyelvezet (pl. assert)

BDD (Behavior Driven Development):

Üzleti viselkedés alapján írjuk a teszteket (pl. Given-When-Then)

Minden szereplő (fejlesztő, tesztelő, üzlet) érti

Cél: közös nyelv, jobb együttműködés
#### ✅ Mi az API tesztelés és miért hasznos?
API tesztelés:
Egy alkalmazás backend interfészeinek (pl. REST, SOAP) ellenőrzése közvetlenül, anélkül, hogy UI-t használnánk.

Hasznossága:

Gyorsabb, mint UI-tesztelés

Stabilabb (nem függ UI változástól)

Korai hibadetektálás a logika szintjén

Automatizálható, CI/CD-ben könnyen használható
#### ✅ Mi az adatvezérelt tesztelés és miért hasznos?
Adatvezérelt tesztelés (Data Driven Testing):
A tesztek bemeneti adatait külső forrásból (CSV, Excel, DB) olvassuk be, így ugyanaz a teszt több adatkombinációval is lefut.

Előnyei:

Tesztlefedettség nő – több eset egyszerűbben lefedhető

Könnyű karbantartás – adatok módosítása nem igényel kódváltozást

Automatizált skálázhatóság







URL: https://chatgpt.com/