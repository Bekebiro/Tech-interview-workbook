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
    | Tesztelési módszerek| Statikus és dinamikus tesztelés kombinációja.          | Elsősorban végső, dinamikus tesztelés.           | Automatikus és manuális tesztelés iterációkban.|
 

<img src="https://t4.ftcdn.net/jpg/03/90/15/65/360_F_390156585_8w1lsOyICIAOvDCU8tExXW2QwLCOFwXD.jpg" alt="image" width="550" height="400">


<img src="https://i.imgur.com/S38EBJw.png" alt="image" width="550" height="400">   <img src="https://segedletek.level14.hu/assets/img/modszertan-vizeses.svg" alt="image" width="550" height="400">


<img src="https://promanconsulting.hu/wp-content/uploads/2022/03/agilis-modszertanok-optimized.jpg" width="550" height="400">
