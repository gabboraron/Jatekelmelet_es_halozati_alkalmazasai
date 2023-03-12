# Játékelmélet és hálózati alkalmazásai

*Csercsik Dávid* - [ITK PPKE](https://itk.ppke.hu/)

## I. - bevezetés
### Előzmények:

> **[Kojima et.al. Matching with couples: Stability and incentives in large markets](https://dash.harvard.edu/bitstream/handle/1/30831454/w16028.pdf)**
>
> A "Matching with Couples: Stability and Incentives in Large Markets" című írás a játékelmélet alkalmazásáról szól a piacokon létrejövő partnerválasztási mechanizmusok vizsgálatára. Az írás az ún. stabil házasság problémáját (stable marriage problem) tárgyalja, amely egy jól ismert matematikai probléma, amelyet a játékelmélet széles körben alkalmaz a piacok és a társadalmi mechanizmusok elemzésére.
>
> Az írás a stabil házasság problémáját általánosítja arra az esetre, amikor a piacok nagyok és a résztvevőknek több preferenciájuk van. Az írás a következő kérdésekre keresi a választ:
> - Mi az optimális partnerválasztási mechanizmus a nagy piacokon, ahol a résztvevőknek több preferenciájuk van?
> - Milyen ösztönzőket lehet bevezetni, hogy az egyes résztvevők a lehető legjobb partnert találják?
> - Milyen stabilitási feltételek szükségesek ahhoz, hogy a partnerválasztási mechanizmus stabil és kielégítő legyen minden résztvevő számára?
>
> Az írás azt vizsgálja, hogy a hagyományos stabil házasság problémájának megoldása hogyan alkalmazható a nagy piacokra, ahol a résztvevőknek több preferenciájuk van. Az írás bemutatja az algoritmusokat és mechanizmusokat, amelyeket alkalmaznak a nagy piacokon, valamint a különböző ösztönzőket, amelyeket bevezethetnek a résztvevők számára, hogy javítsák az eredményeket.
>
> Az írás fontos eredménye, hogy bemutatja az összefüggést a piaci méret és az eredmények minősége között, amelynek eredményeként javaslatokat tesz arra, hogy a résztvevőknek milyen ösztönzőket kell alkalmazniuk a lehető legjobb partnerek megtalálása érdekében. Az írás rámutat arra is, hogy a nagy piacokon a résztvevők nem tudják egyedül megoldani a stabil házasság problémáját, és hogy egy központi szerveződésre van szükség a megfelelő partnerek kiválasztásához. Néhány javaslatuk a következő:
>
> 1. Központi szervezés: Az írás rámutat arra, hogy a nagy piacokon a résztvevőknek nehéz egyedül megoldani a stabil házasság problémáját, és javasolja a központi szervezést. Ezzel biztosítható, hogy a piac minden résztvevője megtalálja a lehető legjobb partnert.
> 2. Ösztönzők bevezetése: Az írás azt javasolja, hogy a résztvevőknek ösztönzőket kell adni a lehető legjobb partner megtalálása érdekében. Ezek az ösztönzők lehetnek pénzügyi juttatások vagy más jutalmak, amelyeket a résztvevők akkor kapnak meg, ha sikeresen megtalálják a megfelelő partnert.
> 3. Részvételi feltételek: Az írás hangsúlyozza a résztvevők részvételi feltételeinek fontosságát a partnerválasztási mechanizmusban. Azt javasolják, hogy a résztvevőknek pontosan definiált feltételek szerint kell részt venniük a partnerválasztásban, és biztosítani kell, hogy mindenki számára ugyanazok a lehetőségek álljanak rendelkezésre.
> 4. További kutatások: Az írás rámutat arra, hogy további kutatásokra van szükség a partnerválasztási mechanizmusok jobb megértése és javítása érdekében a nagy piacokon. Ez magában foglalhatja az új matematikai modellek kidolgozását és az új ösztönzők hatékonyságának vizsgálatát.
>
> *Az összefoglalót a chatGPT generálta 2023/03/11 -án*

> **Cournot competition**
>
> - There is more than one firm and all firms produce a homogeneous product, i.e. there is no product differentiation
> - Firms do not cooperate, i.e. there is no collusion
> - Firms have market power, i.e. each firm’s output decision affects the good’s price
> - Firms compete in quantities, and choose quantities simultaneously
> - The firms are economically rational and act strategically, usually seeking to maximize profit given their competitors’ decisions
> - The number of firms is fixed

### Modern játékelmélet:

> **[Theory of Games and Economic Behavior (1944), Neumann J., Morgenstern O](https://uvammm.github.io/docs/theoryofgames.pdf)** 
> 
> *Magyar összefoglaló KÓCZY Á. LÁSZLÓ által: [A Neumann-féle játékelmélet](http://epa.oszk.hu/00000/00017/00122/pdf/02koczy.pdf)*
>
> A cikk bemutatja a játékelmélet alapjait, azaz a játékok definícióját, a játékosok stratégiáit, a kimenetek valószínűségeit és a játék elméleti megoldásainak koncepcióját.
>
> A cikk bemutatja az összes lehetséges játékot és stratégiákat a játékosok közötti versengés során, és azt is felvázolja, hogyan lehet meghatározni a nyerési stratégiákat minden játékban. Ezenkívül a cikk bemutatja a klasszikus gazdasági problémákat, például a monopolizálást, az oligopóliumokat és az árversenyt, és azt is kifejti, hogy ezek a problémák hogyan értelmezhetők játékelméleti szempontból.
>
> A cikk hatása a gazdaságtanra és a játékelméletre jelentős volt. Az alapelvek, amelyeket a cikk kidolgozott, segítették a közgazdászokat abban, hogy jobban megértsék az emberi döntéshozatali folyamatokat, és hogy jobban fel tudják mérni a gazdasági és üzleti döntések következményeit. A cikk azóta is alapvető olvasmány a játékelmélet és a gazdasági viselkedéselmélet területén
>
> *Az összefoglalót a chatGPT generálta 2023/03/11 -án*

> **Nash-egyensúly (Nash)**
>
> A játékelméletben Nash-egyensúlynak nevezzük a részt vevő játékosok egyéni stratégiáinak olyan stratégiaegyüttesét, amelyre igaz, hogy minden egyes játékos aktuális stratégiája egy parciálisan legjobb választ ad a többi játékos aktuális stratégiájára.
> 
> [wikipedia](https://hu.wikipedia.org/wiki/Nash-egyens%C3%BAly)

> **Részjáték tökéletes egyensúly (Selten)**
>
> A dinamikus játékokban használt Nash-egyensúly egy finomított verziója. Egy stratégiaprofil akkor részjáték-tökéletes egyensúly, amennyiben az eredeti játék minden részjátékában Nash-egyensúlyt indukál. A gyakorlatban ez azt jelenti, hogy ha (1) a játékosok lejátszottak egy olyan játékot, amely mindössze egy részét képezte egy nagyobb játéknak, és (2) a viselkedésük egy Nash-egyensúlyt hoz létre a kisebb játék során, akkor a tevékenységük részjáték tökéletes egyensúlya a nagyobb játéknak. Ismert, hogy minden véges játéknak van részjáték-tökéletes egyensúlya. [*wikipedia*](https://hu.wikipedia.org/wiki/R%C3%A9szj%C3%A1t%C3%A9k-t%C3%B6k%C3%A9letes_egyens%C3%BAly)

> **Shapley-érték**
>
> A shapley érték célja, hogy egy olyan valós számot határozzon meg, hogy egy játékos számára mekkora az értéke annak, hogy részt vesz a játékban. [*N-személyes játékok - Bársony Alex*](http://www.inf.u-szeged.hu/~london/Jatek16/BarsonyA-n-player.pdf)

> **Fogolydilemma**
>
> Azt vizsgálja, hogy két személy közötti együttműködés vagy versengés közötti döntés hogyan befolyásolja az eredményeket. A probléma az alábbi példán keresztül mutatható be:
>
> *Két bűnözőt tartóztatnak le, és a rendőrség külön-külön hallgatja ki őket. Az ügyész azt ajánlja mindkettőjüknek, hogy valljon be, és cserébe könnyebb büntetést kapnak. Azonban ha egyikük beismeri, a másik pedig nem, akkor az előbbi személy kapja a legenyhébb büntetést, míg az utóbbi hosszabb börtönbüntetést kap.*
>
> A Fogolydilemma azt mutatja be, hogy mindkét bűnöző számára a legjobb megoldás az lenne, ha mindketten bevallanák a bűncselekményüket, így mindkettőjük büntetése enyhébb lenne. Azonban ha egyikük sem vall be, akkor semmilyen büntetést nem kapnak. Ebből következik, hogy ha mindkét fél önző és csak a saját érdekeit tartja szem előtt, akkor mindketten rosszabb helyzetben lesznek, és hosszabb börtönbüntetést kapnak.
>
> A Fogolydilemma fontos példa a játékelméletben, mert rámutat arra, hogy az önző cselekvés nem mindig vezet a legjobb eredményre. A probléma megoldása lehet az, ha a két fél közötti együttműködés és bizalom növekszik, vagy ha bevezetnek egy olyan rendszert, amely ösztönzi a kooperációt.
>
> *Az összefoglalót a chatGPT generálta 2023/03/11 -án*

> **Nemteljes információs Bayes-i játékok (Harsányi)**
>
> A Bayes-i játékok olyan játékok, amelyekben a játékosok nem rendelkeznek teljes információval a játékmenetről, és ennek hiányában valószínűségi értékeket adnak a játékmenet lehetséges kimeneteleire.
>
> Harsányi kutatása arra összpontosít, hogy a játékosoknak hogyan kell kezelniük az információ hiányát a játék során. Az írásban Harsányi a játékosok két típusát különbözteti meg: azokat, akiknek teljes információ áll rendelkezésre a játékmenetről, és azokat, akiknek csak részleges információ áll rendelkezésre.
>
> Harsányi rámutat, hogy a részleges információval rendelkező játékosoknak meg kell határozniuk azokat a stratégiákat, amelyekkel az információ hiányát kezelni tudják. A játékosoknak meg kell határozniuk a játékosok lehetséges stratégiáit, az esélyeiket és azokat az információkat, amelyekkel a stratégiájukat módosíthatják.
>
> Harsányi megoldása az volt, hogy a játékosokat valószínűségi eloszlásokkal kell modellezni, amelyek az információ hiányát tükrözik. Ez lehetővé teszi a játékosok számára, hogy becsléseket készítsenek a játékmenet lehetséges kimeneteleiről, és ezeket felhasználják a stratégiájuk meghatározásához.
> 
> A Nemteljes információs Bayes-i játékok című írás tehát arra keresi a választ, hogy a részleges információval rendelkező játékosok hogyan tudják hatékonyan kezelni az információ hiányát a játék során, és hogyan tudják az információkat felhasználni a stratégiájuk meghatározásához.
>
> *Az összefoglalót a chatGPT generálta 2023/03/11 -án*

> **Kooperatív játékok (Aumann, Schmeidler)**
>
> A kooperatív játékok olyan játékok, amelyekben a játékosok csoportokba állnak össze, és közösen dolgoznak ki stratégiákat annak érdekében, hogy a csoport számára optimális eredményt érjék el.
>
> Az írás célja, hogy bemutassa a kooperatív játékok elméleti alapjait, valamint a kooperatív játékokra vonatkozó legfontosabb fogalmakat és definíciókat. Az írásban az autókölcsönző példáját használják fel arra, hogy érzékeltessék, milyen döntéseket hoznak a játékosok, amikor együttműködnek egy csoportban.
> 
> A cikkben szerepel az ún. kooperatív játékoknak a koalíciókra és azok stabilitására vonatkozó elmélete is, amelynek célja, hogy meghatározza, hogy mely koalíciók stabilak és melyek instabilak. Ezt a stabilitási fogalmat aztán használják fel arra, hogy meghatározzák a kooperatív játékokra vonatkozó alapvető fogalmakat, például a koalíció-érték függvényt és az úgynevezett Shapley-értéket, amelyek alapján meghatározható, hogy egy csoportnak milyen mértékben illeti meg az összes játékban felhalmozott jutalom.
>
> Az Aumann és Schmeidler által írt "Kooperatív játékok" című cikk tehát azonban nem csak a kooperatív játékok alapfogalmait és alapelveit mutatja be, hanem részletesen kifejti a koalíciók stabilitására vonatkozó elméletet is, amely azóta is fontos szerepet játszik a kooperatív játékok elméletében.
>
> *Az összefoglalót a chatGPT generálta 2023/03/11 -án*

**Főbb ágak**
- Nem kooperatív játékok (Fogolydilemma, alkujátékok)
- Kooperatív játékok (Szavazás, elosztási problémák)
- Algoritmikus játékelmélet (Párosítás, aukciók)
- Evolúciós játékelmélet (Populációdinamika)
- Kombinatorikus játékok (Sakk és más táblajátékok)

> *In 1985, when Americans were asked how many close friends they had, the most common answer was "three". In 2004, the most common answer was "zero". We now have fewer friends across class, racial, economic, and political lines, because we have fewer friends -- period. And as you just discovered for yourself, the fewer "repeat interactions" there are, the more distrust will spread.* [ NICKY CASE -  "THE EVOLUTION OF COOPERATION (http://ncase.me/trust/)"](http://ncase.me/trust/)

### Racionalitás
A közgazdaságtanban és játékelméletben gyakran felteszik, hogy a résztvevők tökéletesen racionálisak. Azaz, a saját hasznosságukat szeretnék maximalizálni, ennek érdekében képesek tetszőlegesen komplex eszmefuttatásokra és ismerik a lehetséges kimeneteleket és a számukra legkedvezőbbet választják ezek közül.

**A racionalitás korlátai:**

> **Oroszlánok és az altatózott hús**
>
> Egy mesebeli szigeten 15 tökéletes logikával megáldott oroszlán él. Mind nagyon éhesek. Egy napon a szigetre ledobnak egy altatóval átitatott húst. Ha egy oroszlán megeszi, akkor maga is altatóval átitatott hússá válik, amit a többiek megehetnek. Ezt mindegyikük tudja és azt is, hogy a ledobott hús altatózott. Mindent megtesznek azért, hogy éhségüket csillapítsák, ugyanakkor elpusztulni sem akarnak. Mi történik és miért? (A hús oszthatatlan, egy oroszlán vagy megeszi, vagy nem bántja!)
>
> Ha egy oroszlán van, akkor az megeszi a húst. Ha két oroszlán van, akkor egyik sem eszi meg a húst. Ha valamelyik megenné, akkor a másik egyedül maradna
egy altatós hússal, s jóízüen elfogyasztaná. Ha három oroszlán van, akkor az első megeszi a húst, a másik kettö tehetetlenül nézi. Amikor a legfürgébb megette a
húst, a másik kettő ott marad az altatós hússal, s az elöbb tisztázottak szerint nem ennék meg. ...

**Common Knowledge**
- Én tudom, te tudod.
- Én tudom hogy te tudod, te tudod hogy én tudom.
- Én tudom hogy te tudod hogy én tudom...

A Common Knowledge nem triviális következményeit a játékelméletben (*Az összefoglalót a chatGPT generálta 2023/03/11 -án*):
- A koordináció megkönnyítése: Ha a játékosok között közös tudás van egy adott tényről, akkor ez megkönnyíti a koordinációt és növeli az együttműködést. Például, ha két játékos között közös tudás van arról, hogy mindketten ugyanazon játékot játszák, akkor könnyebb számukra koordinálni a stratégiáikat.
- Azt feltételezi, hogy a játékosok érdekelt az információcserében: A Common Knowledge azt feltételezi, hogy a játékosok érdekelték az információcserében, mivel ha egy játékos nem kíváncsi arra, hogy más játékosok mit tudnak, akkor az nem feltétlenül jelenti azt, hogy a játékban szereplő összes játékos tudatában van az adott információnak.
- Lehetővé teszi a bizonytalanság csökkentését: Ha egy játékos tudja, hogy a többi játékos tudja, hogy ő tudja egy bizonyos információt, akkor ez csökkenti a bizonytalanságot, ami lehetővé teszi számára, hogy magabiztosabb döntéseket hozzon.
- Előnyök a kooperatív játékokban: A Common Knowledge fontos szerepet játszik a kooperatív játékokban, mivel a koalíciók közötti együttműködésre van szükség ahhoz, hogy az összes játékos számára optimális eredményt érjenek el.
- Bonyolultság növekedése: Azonban a Common Knowledge fogalma bonyolultabbá is teszi a játékot, mivel az összes játékosnak meg kell értenie, hogy mi a közös tudás, mi az, ami csak egyes játékosok számára ismert, és hogy ez hogyan befolyásolja a stratégiájukat.


**Piros kalap (v Aumann) játék**
- 100 ember ül körbe, mindenkin egy kalap ami kék vagy piros. Mindenki csak a többiekét látja (+ nincs beszéd). Thf h minden kalap piros.
- Egy ceremóniamester a kör közepén bejelenti hogy percenként megüt egy gongot. Miután megüti, ha valaki tudja hogy piros kalap volt rajta, el kell hagynia a termet. (világos hogy a gongütésre senki sem hagyja el a termet - senki nem kap általa új információt)
- Viszont ha az első gongütés előtt kihírdeti hogy ’Legalább 1 piros kalap van a teremben’ (ez nem lep meg senkit hiszem mindenki látja a többi 99 embert piros kalapban)...
- 99 gongütéssig nem történik semmi, de a századikra mindenki feláll és kimegy.

**Az alábbi kritériumok szükségesek ahhoz, hogy a tömeg bölcsessége kiaknázható legyen:**
- a vélemények sokszínűsége
- függetlenség
- decentralizáció (hierarchia hiánya)
- létezzen egy aggregációs mechanizmus

**Ellsberg-paradoxon:**

*’People overwhelmingly prefer taking on risk in situations where they know specific odds rather than an alternative risk scenario in which the odds are completely ambiguous - they will always choose a known probability of winning over an unknown probability of winning even if the known probability is low and the unknown probability could be a guarantee of winning.’* prefer the devil they know

**Ultimátum játék**
- Adott két játékos. Az egyiknek felajánlanak egy összeget (pl. 10$), amit valamilyen arányban megoszthat a másik játékossal. Ha azonban a második játékos kevesli a rá jutó részt, akkor megvétózhatja az elosztást. Ekkor egyikük sem kap semmit.
- Játékelmélet: A második játékos hasznot maximalizál ezért bármilyen keveset is kap elfogadja. Az első játékos ezt felismerve a lehetőlegkevesebbet adja.
- Valóság: A legtöbb játékos elfelezi a kapott pénzt. Az összeg 30%-nálkisebb ajánlatokat rendszerint visszautasítják.

**Diktátor játék**
- Adott két játékos. Az egyiknek felajánlanak egy összeget, amit valamilyen arányban megoszthat a másik játékossal. A második játékosnak semmilyen beleszólása nincs az elosztásba.
- Játékelmélet: A diktátor hasznot maximalizál, ezért semmit nem ad a másiknak.
- Valóság: A legtöbb játékos az összeg 30%-át továbbadja.

**Bizalom játék**
- Adott két játékos. Az egyik kap egy összeget, amit valamilyen arányban megoszthat a másik játékossal. A második játékos az átadott pénz háromszorosát kapja, amiből valamennyit visszajuttathat, ha úgy dönt.
- Játékelmélet: A második játékos hasznot maximalizál, ezért nem küld vissza semmit. Az első játékos ezt felismerve nem ad semmit.
- Valóság: A legtöbb játékos több mint az összeg felét átküldi. Általában legalább ennyit vissza is küldenek

**Bizalom játék (variáns)**
- Adott négy játékos, akik csak számítógépen keresztül tudnak kommunikálni. Mindegyiküknek adnak egy fix zsetonmennyiséget, amit később pénzre válthatnak. Dönthetnek, hogy a zsetonjukból valamennyit a közösbe raknak. A közösben lévő zsetonmennyiséget a játék végén megduplázzák és négy felé osztják. Tehát ha mindegyikük kooperál, akkor megduplázzák a pénzüket, míg ha csak egyvalaki, akkor az elveszíti a berakott pénzének a felét
- A résztvevők 13%-a mindig kooperált, 20%-uk potyautasként viselkedett, a maradék pedig a társai viselkedésétől függően cselekedte az előbbit, vagy az utóbbit.
- Hosszú távon mindenki ugyanolyan jól járt (kialakult az egyensúly).
- Később tesztjátékokon megfigyelték, hogy a játékosok konzisztensen ugyanazon stratégiák mentén hoztak döntéseket, tehát ’programozottan’ cselekedtek
