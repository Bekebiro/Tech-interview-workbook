# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

#### ✅ Mi a tesztelés célja? Mi nem az?

    A tesztelés céljai:
    A munkatermékek, mint például a követelmények, felhasználói történetek, műszaki tervek és kód 
    hibamegelőzés céljából történő kiértékelése

    Annak igazolása, hogy az összes meghatározott követelmény teljesült-e

    Annak ellenőrzése, hogy a teszt tárgya teljes mértékben implementálásra került, továbbá annak, 
    validálása, hogy a felhasználók, illetve más érintett felek elvárásainak megfelelően működik.

    A teszt tárgyának minőségébe vetett bizalom kiépítése

    A meghibásodások és hibák megtalálása és ezáltal a nem megfelelő szoftverminőség kockázati 
    szintjének csökkentése

    Megfelelő információ biztosítása az érintett feleknek, hogy ezáltal megalapozott döntést 
    hozhassanak különösen a teszt tárgyának minőségi szintjére vonatkozóan

    A szerződésben foglalt, jogi vagy szabályozott követelményeknek, szabványoknak való 
    megfelelés biztosítása, és/vagy igazolni a teszt tárgyának ezen követelményeknek, 
    szabványoknak való megfelelőségét

    Komponenstesztelés során egy cél lehet a lehető legtöbb meghibásodás előidézése annak 
    érdekében, hogy az őket okozó hibákat azonosítsák és hamar kijavítsák. Egy másik cél lehet a 
    komponenstesztek kód lefedettségének növelése. 

    Elfogadási tesztelés során a cél lehet annak igazolása, hogy a rendszer az elvárásoknak 
    megfelelően működik és teljesíti a követelményeket. Egy másik célja lehet az érintett felek 
    informálása arról, hogy egy adott időpontban milyen kockázattal járna a rendszer kiadása.

#### ✅ Mik a tesztelési alapelvek?

    A tesztelés alapelvei:

    1. A tesztelés a hibák jelenlétét mutatja, nem a hiányukat
    A tesztelés kimutathatja a hibák jelenlétét, de azt nem képes igazolni, hogy nincsenek hibák. A teszteléssel 
    csökken annak az esélye, hogy a szoftverben felfedezetlen hibák maradnak, de ha nem találnak hibát, az 
    nem bizonyítja, hogy a rendszer helyes.

    2. Nem lehetséges kimerítő teszt
    Kimerítő teszt, azaz a mindenre (a bemenetek és előfeltételek minden kombinációjára) kiterjedő tesztelés a 
    triviális eseteket leszámítva nem lehetséges. Ahelyett, hogy megkísérelnénk a kimerítő tesztelést, 
    kockázatelemzés, tesztelési technikák használata és priorizálása szükséges a tesztelési erőforrások 
    összpontosításához.

    3. A korai tesztelés időt és pénzt spórol
    A hibák korai megtalálásának érdekében a szoftverfejlesztési életciklus során mind a statikus, mind a 
    dinamikus teszttevékenységeket a lehető legkorábban el kell kezdeni. A korai tesztelésre az angol 
    szakirodalomban néha shift left-ként utalnak. A szoftverfejlesztési életciklus alatti korai tesztelés segít a 
    költséges változtatások csökkentésében vagy eliminálásában. 

    4. Hibafürtök megjelenése
    A kiadást megelőző tesztelés során megtalált hibák többsége rendszerint néhány modulban van, vagy ezen 
    modulok felelősek a működési meghibásodások többségéért. A megjósolt hibafürtök és a tesztelés vagy 
    működés során ténylegesen megfigyelt hibafürtök fontos bemenetként szolgálnak a tesztelési erőforrások 
    összpontosítása érdekében alkalmazott kockázatelemzés számára. 

    5. Kísérd figyelemmel a féregirtó paradoxont 
    Ha ugyanazokat a teszteket hajtjuk végre újra és újra, akkor ezen tesztek egy idő után nem fognak új hibákat 
    találni. Ahhoz, hogy új hibákat találjunk, a létező teszteket és tesztadatokat módosítani kell, illetve új teszteket 
    kell írni. (A tesztek egy idő után már nem hatékonyak a hibák megtalálásában csakúgy, ahogyan egy idő 
    után a féregirtók sem hatékonyak a rovarok elpusztításában.) Néhány esetben például az automatikus 
    regressziós tesztelés esetében a féregirtó paradoxonnak egy előnyös kimenete is van, ami a regressziós 
    hibák viszonylag alacsony száma.

    6. A tesztelés függ a körülményektől
    A tesztelést különböző körülmények esetén különbözőképpen hajtják végre. Például egy biztonságkritikus 
    ipari irányító szoftvert másképp tesztelnek, mint egy e-kereskedelmi mobilalkalmazást. Egy másik példában, 
    a tesztelés egy Agilis projektben különbözik egy szekvenciális szoftverfejlesztési életciklust alkalmazó projekt 
    tesztelésétől.

    7. A hibamentesség egy téveszme
    Néhány szervezet azt várja el, hogy a tesztelők minden lehetséges tesztet le tudjanak futtatni és minden 
    lehetséges hibát megtaláljanak, de az 1. és a 2. alapelv kimondja, hogy ez lehetetlen. Továbbá téveszme 
    (téves meggyőződés) azt várni, hogy csupán azzal, hogy sok hibát találnak meg és javítanak ki, biztosítják a 
    rendszer sikerességét. Például a meghatározott követelmények teljeskörű tesztelése és az összes talált hiba 
    kijavítása még mindig eredményezhet egy nehezen használható rendszert, ami nem elégíti ki a felhasználók 
    összes igényét és elvárását, vagy más hasonló rendszerekhez képest silányabb minőségű.

#### ✅ Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?

    A unit teszt lényege, hogy az egységeket külön-külön is tudjuk tesztelni, ezáltal könnyebb a hibakeresés folyamata.

    A tesztelését általában a kódot író fejlesztő végzi.

#### ✅ Mik a tesztszintek, és mi a különbség köztük?

    A tesztszintek teszttevékenységek olyan csoportjai, amelyeket együtt szerveznek és kezelnek.
    Példák:
        komponenstesztelés
        integrációs tesztelés
        rendszertesztelés
        elfogadási tesztelés

    Különbség, hogy minden tesztszinthez a megfelelő tesztkörnyezetre van szükség.

#### ✅ Mi a különbség a verifikáció és a validáció között?

    Verifikációkor a specifikált követelményeknek való megfelelést ellenőrzi
    Validáció során a felhasználói igényeknek való megfelelést ellenőrzi

#### ✅ Mik a tesztelési típusok, és mi a különbség köztük?
    Tesztelési típusok:
        funkcionális tesztelés
        Nemfunckionláis tesztelés
        Fehérdoboz tesztelés
        Ellenőrző tesztelés
        Regressziós tesztelés

    Főbb különbségek:
        Mire fókuszál az adott tesztelés? (funkcionális vagy nemfunkcionális)
        Van amelyik automatizált, míg van amelyik nem
        Más a cél az egyes teszteléseknél

#### ✅ Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?

    Jellemző	       | Fehér doboz	         |   Szürke doboz	       | Fekete doboz
    -------------------|-------------------------|-------------------------|-------------------------
    Rálátás a kódra	   | Teljes	                 |   Részleges	           | Nincs
    -------------------|-------------------------|-------------------------|-------------------------
    Célcsoport	       | Fejlesztők	             |   Fejlesztők, tesztelők | Tesztelők, végfelhasználók
    -------------------|-------------------------|-------------------------|-------------------------
    Fókusz	           | Belső működés	         |   Kombinált nézőpont	   | Külső funkcionalitás
    -------------------|-------------------------|-------------------------|-------------------------
    Alkalmazás szintje | Alacsony szintű tesztek |   Közepes szintű tesztek| Magas szintű tesztek

#### ✅ Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?
    Felhasználói elfogadási tesztelés:
        A felhasználók által a rendszeren végzett felhasználói elfogadási tesztek általában arra irányulnak, hogy 
        valós vagy szimulált éles működési környezetben validálják azt, hogy a rendszer a leendő felhasználók 
        számára alkalmas lesz-e a használatra.

    Rendszertesztelés:
        A teljes rendszer vagy termék viselkedésére és képességeire összpontosít, gyakran 
        figyelembe véve a végpontok közötti feladatokat, amelyeket a rendszer képes végrehajtani, és a 
        nemfunkcionális viselkedéseket, amelyeket ezen feladatok végrehajtása közben mutat.

#### ✅ Sorolj fel különbségeket a regressziós tesztelés, a füsttesztelés és az újratesztelés között!

    Jellemző	       | Regressziós testelés      | Füstteszstelés	           | Újratesztelés
    -------------------|---------------------------|---------------------------|-----------------------------
    Cél    	           | A meglévő funkciók helyes | Alapfunkciók működőképes- | Egy adott hiba kijavításának 
                       |  működésének ellenőrzése  | ségének gyors ellenőrzése.| ellenőrzése.
                       |  változtatások után.      |                           |
    -------------------|---------------------------|---------------------------|-----------------------------                    
    Időzítés           | Funkciófrissítések vagy   |   Új build bevezetésekor. |    Hiba javítása után.
                       | hibajavítások után.       |                           |
    -------------------|---------------------------|---------------------------|-----------------------------
    Fókusz  	       |Széles körű funkciók       | Kritikus funkciók magas   |  Egy adott probléma.
                       | ellenőrzése.|             | szintű tesztelése.        |                
                       |                           |                           |  
    -------------------|---------------------------|-------------------------  |-----------------------------
    Tesztesetek        |   Meglévő tesztek         |  Minimális, alapvető      | Új, specifikus tesztek.
                       |   újrafuttatása.          |    tesztek.               |
                       |                           |                           |
    -------------------|---------------------------|-------------------------  |-----------------------------
    Automatizáció      | Gyakran automatizált.     |Lehet manuális vagy        | Többnyire manuális.
                       |                           | automatizált.             |     

#### ✅ Mi a különbség a statikus és dinamikus tesztelés között?
    
    A statikus tesztelésnek és a dinamikus tesztelésnek lehetnek azonosak a céljai, mint 
    például a munkatermékek minőségének kiértékelése és a hibák lehető legkorábbi azonosítása. A statikus és 
    a dinamikus tesztelés kiegészíti egymást azzal, hogy különböző típusú hibákat találnak meg.
    Az egyik fő eltérés az, hogy a statikus tesztelés a munkatermékekben a hibákat közvetlenül találja meg, 
    ellentétben azzal, hogy a hibák okozta meghibásodásokat azonosítjuk a szoftver futtatása során. A hiba 
    hosszú ideig rejtőzhet egy munkatermékben anélkül, hogy meghibásodást váltana ki. Lehet, hogy az a 
    végrehajtási útvonal, amelyen a hiba elhelyezkedik, csak ritkán hajtódik végre, vagy nehezen érhető el, így 
    nem lesz könnyű olyan dinamikus tesztet létrehozni és végrehajtani, amely találkozik a hibával. A statikus 
    tesztelés sokkal kevesebb erőfeszítés mellett is képes lehet a hiba megtalálására.
    Egy másik különbség lehet az, hogy a statikus tesztelés felhasználható a munkatermékek konzisztenciájának 
    és belső minőségének javítására, míg a dinamikus tesztelés tipikusan a kívülről látható viselkedésekre 
    fókuszál.
    A dinamikus teszteléssel összehasonlítva azok a tipikus hibák, amelyeket könnyebb és olcsóbb statikus 
    teszteléssel megtalálni és javítani, a következőket foglalják magukba:

    • Követelmény hibák (például következetlenségek, többértelműségek, ellentmondások, kihagyások, 
    pontatlanságok és ismétlődések)

    • Tervezési hibák (például nem hatékony algoritmusok vagy adatbázis struktúrák, erős kapcsolódás, 
    kismértékű kohézió)

    • Kódolási hibák (például változók értékadás nélkül, deklarált, de fel nem használt változók, elérhetetlen 
    kód, ismétlődő kód)

    • Szabványoktól való eltérés (nem követi például a kódolási konvenciókat)

    • Helytelen interfész specifikációk (eltérő mértékegységek használata például a hívó rendszerben és a 
    hívott rendszerben)

    • Biztonsági sebezhetőségek (például a puffer túlcsordulás lehetőségei)

    • Hiányok vagy pontatlanságok a tesztbázis nyomonkövethetőségében vagy a lefedettségben (például 
    hiányzó tesztek egy elfogadási feltétel vizsgálatára)

    A karbantarthatósági hibák legtöbb típusa továbbá csak statikus teszteléssel található meg (például a nem 
    megfelelő modularizáció, a komponensek korlátozott újrafelhasználhatósága, nehezen elemezhető és új 
    hibák létrehozása nélkül alig módosítható kód)


### ✅ Hasonlítsd össze a V-modellt, a vízesés modellt és az Agile megközelítést a tesztelés szempontjából!

    | Jellemző            | V-modell                                               | Vízesés modell                                   | Agile megközelítés                             |
    |---------------------|--------------------------------------------------------|--------------------------------------------------|------------------------------------------------|
    | Tesztelés kezdete   | Korán, a fejlesztési fázisokkal párhuzamosan.          | Későn, a fejlesztési folyamat végén.             | Folyamatosan, minden iteráció során.           |
    |---------------------|--------------------------------------------------------|--------------------------------------------------|------------------------------------------------|
    | Tesztelés szerepe   | Minden fejlesztési fázishoz tesztelési fázis tartozik. | Elkülönített, csak a végtermékre vonatkozik.     | A fejlesztési folyamat integrált része.        |
    |---------------------|--------------------------------------------------------|--------------------------------------------------|------------------------------------------------|
    | Rugalmasság         | Merev, jól definiált folyamatokkal.                    | Merev, változtatások nehezen kezelhetők.         | Nagyon rugalmas, gyorsan reagál a változásokra.|
    |---------------------|--------------------------------------------------------|--------------------------------------------------|------------------------------------------------|
    | Hibák észlelése     | Korai fázisban, a követelmények ellenőrzésével.        | Késői fázisban, a teljes rendszer tesztelésekor. | Gyorsan, már az iterációk közben.              |
    |---------------------|--------------------------------------------------------|--------------------------------------------------|------------------------------------------------|
    | Dokumentáció        | Részletes és alapos, minden szakaszhoz kötött.         | Részletes, lineárisan követi a fázisokat.        | Minimális, a funkciók fejlesztésére fókuszál.  |
    |---------------------|--------------------------------------------------------|--------------------------------------------------|------------------------------------------------|
    | Iteráció lehetősége | Nincs iteráció, szigorú szekvencia.                    | Nincs iteráció, szigorú szekvencia.              | Iteratív és inkrementális folyamat.            |
    |---------------------|--------------------------------------------------------|--------------------------------------------------|------------------------------------------------|
    | Csapatmunka         | Szakaszok közötti átadás dominál.                      | Egyirányú kommunikáció a fázisok között.         | Folyamatos csapatmunka és visszacsatolás.      |
    |---------------------|--------------------------------------------------------|--------------------------------------------------|------------------------------------------------|
    | Tesztelési módszerek| Statikus és dinamikus tesztelés kombinációja.          | Elsősorban végső, dinamikus tesztelés.           | Automatikus és manuális tesztelésiterációkban.|


#### ✅ Milyen lépéseket követnél egy hiba megtalálásakor?

        Először pontosan azonosítanám a hibát, magyarul mikor jelenik meg a hiba és milyen hibát okoz az eset. Eztán dokumentálom is a hibát. Megpróbálomn reprodukálni a hibát, hogy valóban egy folyamatosan fennálló hibáról van- e szó, vagy csak egy véletlen hiba történt. Folytatásképpen elkezdem az egységeket külön külön kezelni, hogy megtudjam, mi az ami működik és mi az, ami nem. Miután a hiba megvan, megnézem, hogy volt e a közelmúltban valami változtatás a kódban, esetleg van e valahol logikai hiba. Ha ez is megvan, javítom a hibát és újratesztelek. Ha minden rendben van, elkészítem a dokumentációt.

#### ✅ Beszélj a gyakori tesztjelentésekről és részleteikről!

        A tesztjelentés célja, hogy összefoglalja és átadja a tesztelési tevékenységre vonatkozó információkat a 
        tesztelési tevékenység (például egy tesztszint) során és annak végén. A vizsgálati tevékenység során 
        elkészített tesztjelentést más néven tesztelőrehaladási jelentésnek, míg a tesztelési tevékenység végén 
        elkészített tesztjelentést összefoglaló tesztjelentésnek is nevezik.

        A tipikus összefoglaló tesztjelentések az alábbiakat tartalmazhatják:
            - Az elvégzett tesztelés összefoglalása
            - Tájékoztatás a tesztelési időszak alatt történtekről
            - Eltérések a tervtől, beleértve a tesztelési tevékenységek ütemtervét, időtartamát vagy a ráfordításokat
            - A tesztelés és a termékminőség állapota a kilépési kritériumok vagy a „kész” definíciójának tekintetében
            - Azok a tényezők, amelyek blokkolták vagy továbbra is blokkolják a haladást
            - A hibák, a tesztesetek, a teszt lefedettség, a tevékenység előrehaladása és az erőforrás-fogyasztás mérőszámai 
            - A fennmaradó kockázatok 
            - Újrahasznosítható tesztelési munkatermékek

        A tesztjelentés tartalma a projekttől, a szervezeti követelményektől és a szoftverfejlesztési életciklustól függően változik. A tesztjelentéseknek a projekt kontextusá
        alapuló testre szabása mellett a tesztjelentéseket a jelentés közönségének megfelelően kell kialakítani

#### ✅ Mit tartalmaz egy hibajelentés?

        Mivel a tesztelés egyik célja, hogy hibákat találjon, a tesztelés során talált hibákat rögzíteni kell.

         hibajelentés általában a következőket tartalmazza:
            - Azonosító
            - A bejelentett hiba címe és rövid összefoglalása
            - A hibajelentés dátuma, a kibocsátó szervezet és a szerző
            - A tesztelem (az éppen tesztelt konfigurációs elem) és a környezet azonosítója
            - A fejlesztési életciklus fázisa(i), amelyben a hibát észlelték
            - A hiba reprodukálását és megoldását lehetővé tevő leírás, beleértve a naplófájlokat, az adatbázis mentéseket, képernyőképeket vagy felvételeket (ha volt ilyen a teszt végrehajtása során)
            - Elvárt és tényleges eredmények
            - A hiba súlyosságának (severity) hatóköre vagy mértéke az érdekelt felek érdekeit tekintve
            - A javítás sürgőssége/prioritása
            - A hibajelentés állapota (pl. nyitott, elhalasztott, duplikált, megoldásra váró, ellenőrző tesztelésre váró, újranyitva, lezárt)
            - Következtetések, ajánlások és jóváhagyások
            - Globális problémák, például olyan területek, amelyekre a hibából eredő változás hatással lehet
            - Változási előzmények, mint például a projektcsapat tagjai által a hibával kapcsolatos lépések, hogy elkülönítsék, javítsák és ellenőrizzék azt
            - Hivatkozások, beleértve a problémát feltáró tesztesetet is


#### ✅ Hogyan rangsorolnál egy hibát?

        A hibát két féle kéépen lehet csoportosítani:
            - Súlyosság
            - Prioritás

        Súlyosság alapján:
            - Kritikus (Critical) - A rendszer teljesen használhatatlan (pl. nem indul el).
            - Magas (High) - Fő funkció nem működik, de a rendszer fut.
            - Közepes (Medium) - Másodlagos funkció hibás, kerülőút lehetséges.
            - Alacsony (Low) - Esztétikai vagy kisebb hiba, nincs funkcionális hatása.

        Prioritás alapján:
            - Magas - Azonnali javítást igényel.
            - Közepes -	Hamar javítani kell, de nem kritikus.
            - Alacsony - A javítás ráér, nem sürgős.


#### ✅ Melyik teszteseteket érdemes automatizálni és melyiket nem?

        Tesztesetek, amiket érdemes automatizálni:

            - Gyakran ismétlődő tesztek
                Automatizálva gyorsabb, megbízhatóbb, és nem fárad el, mint az ember.

            - Nagy adat- vagy időigényű tesztek
                Több ezer bemenettel történő tesztelés, tömeges adatfeldolgozás. Automata futtatás ember helyett, pl. éjszaka is.

            - Stabil és kiszámítható funkciók tesztelése
                Nincsenek benne gyakori UI vagy design változások.

            - Integrációs és regressziós tesztek
                Ha egy új fejlesztés visszahatásait vizsgáljuk a meglévő rendszerre. Automatikusan figyelmeztet, ha valami "elromlott".

            - Platformfüggetlen, jól szkriptelhető tesztek
                REST API tesztek, parancssori eszközök tesztelése.

        Tesztesetek, amiket nem éredemes automatizálni:

            - UI/UX vagy vizuális tesztek
                Nehéz automatizálni, szubjektív értékelés szükséges.

            - Egyszeri vagy ritkán használt tesztek
                Automatizálás költsége nagyobb, mint a manuális futtatás haszna.

            - Explorációs tesztelés
                Szabad felfedezés, hibakeresés új funkcióknál, ahol még nincs minden véglegesítve. Tesztelő kreativitása fontosabb, mint az ismétlés.

            - Gyorsan változó funkciók tesztje
                Ha a funkció vagy UI még nem végleges, és gyakran változik. Automatizált tesztek gyakran "eltörnek", így a karbantartásuk túl költséges lenne.



#### ✅ Írj le egy jó automatizált tesztet!

        Egy jó automatizált teszt:
            - Egyértelmű: 
                pontosan meghatározza, mit tesztel.
            - Izolált: 
                ne függjön más teszttől vagy környezeti állapottól.
            - Ismételhető: 
                mindig azonos eredményt adjon azonos körülmények között.
            - Gyors: 
                ehetőleg néhány másodperc alatt fusson le.
            - Olvasható és karbantartható.



#### ✅ Mi a Selenium, Selenium IDE és Selenium WebDriver?

        A Selenium egy nyílt forráskódú tesztautomatizálási keretrendszer, amely lehetővé teszi webalkalmazások automatikus tesztelését különböző böngészőkben és platformokon. Fő célja, hogy utánozza a felhasználói viselkedést (kattintás, gépelés, űrlapküldés stb.), és ezáltal segítse a hibák korai felismerését.

        A Selenium IDE és a Selenium WevDriver egy-egy komponense a Seleniumnak

        Selenium IDE tulajdonságai:

            - Kattintás-alapú tesztfelvevő eszköz: rögzíti a felhasználó interakcióit a weboldallal, és automatikusan generál teszteket.
            - Kódolási ismeret nem szükséges.
            - Egyszerű és gyors, de kevésbé rugalmas és nehezebben karbantartható komplex eseteknél.

        Selenium WebDriver tulajdonságai:

            - A legelterjedtebb és legerőteljesebb Selenium-eszköz.
            - Programozási nyelvekkel használható: Java, Python, C#, JavaScript, stb.
            - Közvetlenül irányítja a böngészőt – valóban úgy működik, mintha egy ember kezelné.
            - Robusztus, rugalmas és bővíthető komplex automatizált tesztelési forgatókönyvekhez.

#### ✅ Hogyan lehet azonosítani a webes elemeket?

        Webes elemek azonosítása az automatizált tesztelés egyik legfontosabb lépése – hiszen ezek segítségével „talál rá” a teszt a gombokra, mezőkre, linkekre, stb. A helyes elem-azonosítás megbízhatóbbá és stabilabbá teszi a teszteket.

        Főbb elem-azonosítási módszerek:

            | Módszer          | Mikor hasznos?                                        | Példa                                              |
            | ---------------- | ----------------------------------------------------- | -------------------------------------------------- |
            | **ID**           | Egyedi azonosító, ha van                              | `driver.find_element(By.ID, "login-button")`       |
            | ---------------- | ----------------------------------------------------- | -------------------------------------------------- |
            | **Name**         | Űrlapmezőknél gyakori                                 | `By.NAME, "email"`                                 |
            | ---------------- | ----------------------------------------------------- | -------------------------------------------------- |
            | **Class name**   | Stílusazonosító – nem mindig egyedi                   | `By.CLASS_NAME, "btn-primary"`                     |
            | ---------------- | ----------------------------------------------------- | -------------------------------------------------- |        
            | **Tag name**     | HTML címke (ritkán önmagában elég)                    | `By.TAG_NAME, "input"`                             |
            | ---------------- | ----------------------------------------------------- | -------------------------------------------------- |
            | **Link text**    | Kattintható linkekhez (a teljes link szövege alapján) | `By.LINK_TEXT, "Kijelentkezés"`                    |
            | ---------------- | ----------------------------------------------------- | -------------------------------------------------- |
            | **Partial link** | Linkekhez, ha csak a szöveg egy része ismert          | `By.PARTIAL_LINK_TEXT, "Kijel"`                    |
            | ---------------- | ----------------------------------------------------- | -------------------------------------------------- |
            | **CSS selector** | Precíz, gyors, jól testreszabható                     | `By.CSS_SELECTOR, "div.form > input[type='text']"` |
            | ---------------- | ----------------------------------------------------- | -------------------------------------------------- |
            | **XPath**        | Nagyon rugalmas, komplex szerkezetekhez is jó         | `By.XPATH, "//button[@id='login-button']"`         |


#### ✅ Hogyan lehet várni az elemekre, és mi lehet a probléma? Gyűjtsd össze a lehetséges hibákat és okokat!

#### ✅ Hasonlítsd össze a POM és a Keyword Driven Testing megközelítéseket!

#### ✅ Mi a különbség a TDD és BDD között?

#### ✅ Mi az API tesztelés és miért hasznos?

#### ✅ Mi az adatvezérelt tesztelés és miért hasznos?
 

<img src="https://t4.ftcdn.net/jpg/03/90/15/65/360_F_390156585_8w1lsOyICIAOvDCU8tExXW2QwLCOFwXD.jpg" alt="image" width="550" height="400">


<img src="https://i.imgur.com/S38EBJw.png" alt="image" width="550" height="400">   <img src="https://segedletek.level14.hu/assets/img/modszertan-vizeses.svg" alt="image" width="550" height="400">


<img src="https://promanconsulting.hu/wp-content/uploads/2022/03/agilis-modszertanok-optimized.jpg" width="550" height="400">
