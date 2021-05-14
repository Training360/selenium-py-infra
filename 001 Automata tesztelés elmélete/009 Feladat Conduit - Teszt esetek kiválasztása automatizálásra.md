# 009 Feladat Conduit - Teszt esetek kiválasztása automatizálásra

A feladatod, hogy lokálisan elindítsd a Conduit app-ot a saját gépeden. A sajét forkodban dolgozz kérlek. Nézzd meg újra az ide vonatkozó videókat, ha nem tiszta, hogy hogyan kell a fork-ot létrehozni. 
Az indításhoz használd a docker-compose file-t ami a projekttel érkezik.

Addott pár teszteset a Conduit app-hoz. 
Ezeket itt találod meg: [https://drive.google.com/drive/folders/1CPilqJvJkAbi3QloM6SKJkxjQY00coLC](https://drive.google.com/drive/folders/1CPilqJvJkAbi3QloM6SKJkxjQY00coLC)

//TODO további teszt esetekkel bővíteni

Ezek közül a tesztesetek közül melyikre készítenél és milyen automatizált tesztet? Miért? 

A saját forkodban készíts kérlek egy `docs` mappát és ebbe készíts egy `docs/selected_for_automation.txt` fájlt. Ebbe sortörésekkel sorold fel a felfedezett önáló funkciókat.

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

Minden tesztesetre reagálj.