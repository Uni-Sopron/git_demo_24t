# EasyOS

## Hard drivera telepítés
Nulladik lépésként el kell döntenünk, hogy melyik drive-unkra szeretnénk
telepíteni az operációs rendszert. Lehet egy teljesen üresre, vagy
olyanra is, amin már van másik oprendszer. Egyszerűbb dolgunk van, ha a
teljes drive-ot nekiszenteljük, de nem sokkal bonyolultabb a megosztott
sem, mivel az EasyOS képes létezni a többi oprendszer mellett.
Az én esetemben (a gyakorlás végett) egy megosztott hard drive-ot
kapott, azonban nem szerepel semmi más rajta.
Elsőként létre kellett hoznom egy üres teret, amit az ntfs partíció
csökkentésével értem el. Ez után ahhoz, hogy vfat esp és ext4 partíciót
hozzak létre, Linux alapú oprendszerre volt szükségem, úgyhogy
letöltöttem a Win32DiskImager nevű programot, ami a .img fájlt átírta a
hard drive-ra, ami ezáltal létrehozott egy boot partíciót, ami azért
felelős, hogy a boot menüben megjelenjen és kiválasztható legyen az
EasyOS, illetve lérehozott még egy ext 4 partíciót is, ami sokszorosan
nagyobb az előbbinél, mivel ebben van maga az operációs rendszer setupja.
Mindezek után újra kellett indítanom a gépet, bemenni a boot menübe és
beállítani a lehetőségek között, hogy hard drive-ról is bootolhasson.
Mikor ez megvolt, bootolhattam EasyOS-ben, ahol már csak a setupot
kellett megcsinálnom, ahol beállítottam a felhasználót.
Egy újraindítás után személyre szabtam a billentyűzetet, a nyelvet, a
tűzfalat, illetve az időt, és ezzel be is fejeződött a telepítést és a setup.
## Virtuális gépre telepítés
Nulladik lépésként le kell tölteni az EasyOS lemezképfájlját.