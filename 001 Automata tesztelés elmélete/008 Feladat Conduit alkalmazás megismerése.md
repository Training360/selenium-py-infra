# 008 Feladat Conduit alkalmazás megismerése

A feladatod, hogy lokálisan elindítsd a Conduit app-ot a saját gépeden. 

## Github Fork

Nyílt forráskódú projekt esetében előfordul, hogy más kódjához mi magunk is hozzá szeretnénk nyúlni, szeretnénk bele fejleszteni, ki szeretnénk egészíteni. Érthető okokból azonban a projektek tulajdonosai nem adnak bárkinek hozzáférést a repóhoz. Emiatt szükség lesz egy saját változatra.

Megtehetjük azt, hogy saját magunk leklónozzuk a projektet, majd módosítva a “remote” beállításokat egy saját, üres repóba feltöltjük. Ezt hívjuk a repó fork-olásának (a szó azt jelenti, hogy elágazás: ahogy az út egyből kettéágazik, vagy ahogy a villa egy nyeléből több kisebb “ág” nő ki).

Ha a platform megengedi, akkor ezt egy kattintással is elvégezhetjük. A példában a GitHub weboldalt használom.

### Forkolás
A Fork gomb csak akkor jelenik meg a Github weboldalon, ha:
 * ezt nem tiltotta le az eredeti projekt gazdája
 * be vagy jelentkezve a saját felhasználóneveddel és jelszavaddal a Github.com-on.

A projekt weboldalán kattintsunk erre a gombra:

![image](https://user-images.githubusercontent.com/227298/120960768-d0447c80-c75c-11eb-8832-d6355b25ac6a.png)

Ez után a saját projektjeink között meg fog jelenni a repó, együtt a teljes történelmével, változtatásaival.

A kapcsolat nem szűnik meg a két repó között, a név alatt látszik, hogy melyik volt az eredeti repó:

![image](https://user-images.githubusercontent.com/227298/120960826-eb16f100-c75c-11eb-86dc-9109404bb9e8.png)

Forkolás után a két projektet különbözőnek lehet tekinteni, a saját repónkba gond nélkül tudunk saját kódot push-olni - de ha szeretnénk, akkor az eredetit is nyomon tudjuk követni, néhány parancs kiadásával az eredeti projekt változtatásait is tudjuk integrálni.

Ilyen módon lehet karban tartani pl. egy népszerű, Linux-os projekt Windows-os változatát, ha az eredeti készítő erre nem tud időt szánni:

Az eredeti projekt a Linux-os kódot tartalmazza
A forkolt projekt tartalmazza a szükséges Windows-os módosításokat, miközben naprakészen tud maradni az eredetivel
A két projekt innentől kezdve párhuzamosan fut.

Alkalomszerűen előfordulhat, hogy a fork-olt projekt válik népszerűbbé, mert az eredeti tulajdonosánál jobban karban tartja, gyorsabban fejleszti az új funkciókat stb. Ez történt az OpenOffice esetében is: az eredeti projekt jövőjét féltették az Oracle-től, ezért készítettek a fork-ot, a jogi problémákat elkerülendő a projektet átneveztét LibreOffice-re, és azóta ez lett a népszerűbb változat.

### Pull request
Ha a saját módosításunkat az eredeti projekt fejlesztői is szívesen látnának, akkor készíthetünk egy ún. pull request-et. Ez egy felkérés arra, hogy bizonyos commitokat az eredeti fejlesztő pull-oljon a mi projektünkből. Ezt ő pedig elfogadhatja, vagy visszautasíthatja.

Példa egy [pull request-re](https://github.com/dotnet/roslyn/pull/31801): lehet comment-elni, látszanak a bele tartozó commitok.

Github-on a pull request az elsődleges módszer a különböző fejlesztők közös munkájához. Cégen belüli, privát git repók esetében is léteznek hasonló funkciók, amely egy repón belül, a különböző fejlesztési ágak között valósítja meg ugyanezt (ún. merge request - merge-elésre felkérés).

## Munka a Conduit alkalmazással
Hozz létre egy Github forkot (ha már van fiókod az is jó) és innen végig a saját másolatodban dolgozz kérlek. 

Itt találdo az eredeti Conduit repo-t: https://github.com/tjozsa/conduit

Az indításhoz használd a docker-compose file-t ami a projekttel érkezik. A leírást a lemásolt repo README.MD-jében találod.

A feladatod az lesz, hogy fedezzd fel az alkalmazás képességeit. A saját forkodban készíts kérlek egy `docs` mappát és ebbe készíts egy `docs/functions.txt` fájlt. 

Most még használhatod a Forkod Github-os web felületét mappák és fileok feltöltésére/szerkesztésére, de később a Git/Github résznél a saját gépeden is megtanulod majd szerkeszteni ezeket a repokat.

Ebbe sortörésekkel sorold fel a felfedezett önáló funkciókat.

PL:
```
regisztráció: az alkalmazásba be lehet regisztrálni, név, emailcím és jelszó megadásával
bejelentkezés: az alkalmazásba be lehet jelentkezni egy meglévő felhasználói fiókkal
...
```

Legalább még 8 funkciót írj össze.
