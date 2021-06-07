# 009 Feladat Conduit - Teszt esetek kiválasztása automatizálásra

A feladatod, hogy készíts az előzőleg összeírt funkciókhoz manuális teszteseteket. Ha kell nézzd vissza a 0. hét videós konzultációit.

Használd a nulladik héten megosztott Teszteset sablon-t ha nincs jobb formátum amit használni tudnál.

Futtasd le a teszeseteket a manuális lokálisan futó Conduit applikáción.

Az elkészült teszteseteketek kérlek készíts egy mappát a saját forkodban már előzőleg elkészített `docs` mappánban: `docs/testcasses`. Ebbe a mappába add hozzá az összes testcase-t amit készítettél.

## Kérdések amiket meg kell válaszolnod 
Ezek közül a tesztesetek közül melyikre készítenél és milyen automatizált tesztet? Miért? 

A saját forkodban készíts egy `docs/selected_for_automation.txt` fájlt. Ebbe sortörésekkel sorold fel a felfedezett önáló funkciókat.

Most még használhatod a Forkod Github-os web felületét mappák és fileok feltöltésére/szerkesztésére, de később a Git/Github résznél a saját gépeden is megtanulod majd szerkeszteni ezeket a repokat.

PL:
```
A001,CON_TC_004_login, felület automatizázás, mert ismételt végrehajtást tartalmaz
...
```
Ahol:
* `A001` azt jelenti, hogy ezt automatizálod elsőnek, tehát sorszám.
* `CON_TC_004_login` az eredeti manuális teszteset azonosítója
* `felület automatizázás` | `API teszt` | `egyéb teszt` egyike a felsoroltaknak
* a legutolsó elem a szöveges magyarázat, lehetőleg egy mondatban.

Minden tesztesetre reagálj. Az is válasz, ha azt írod, hogy nem automatizálható, mert ...
