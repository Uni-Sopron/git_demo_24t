# Raspberry Pi OS - Telepítési dokumentáció
## Raspberry Pi OS-ről röviden
>A Raspberry Pi OS egy hivatalos, Debian alapú operációs rendszer, amelyet kifejezetten a Raspberry Pi miniszámítógépekhez terveztek. Könnyen használható grafikus felületet kínál, és támogatja a tanulást, a programozást, valamint különféle projektek megvalósítását. Ideális választás kezdőknek és haladó felhasználóknak egyaránt.

## Telepítés Oracle VirtualBoxban 
1. ### Lemezkép letöltése 
    A lemezképet a Raspberry hivatalos oldaláról tudjuk letölteni a következő linken: [raspberrypi.com](https://www.raspberrypi.com/software/operating-systems/)
    
    PC-hez csak 32 bites verziót tudunk letölteni (Raspberry Pi OS (Legacy) with desktop)

2. ### Virtuális gép létrehozása
    1. Virtualboxon belül kattintsunk a "New" gombra. A gombot tartalmazó menüt az alkalmazásban felül, középen találjuk.
    ![new](images/new.png)

    2. Virtuális gép beállítása
    * Name andy Operating System 
        * "Name" menüpontban meg kell adnunk a gép nevét, ami esetünkben Raspberry_Pi_OS lesz.<br>
        * "Folder"-nél meg kell adnunk, hogy a host számítógépen hova hozzuk létre a vm mappáját.<br>
        * "ISO Image"-hez válasszuk ki az OS lemezképét
        * "Type"-nál Linux-ot kell választani
        * "Version"-nél pedig Debian 11 Bullseye (32-bit)-et válasszunk

    ![settings1](images/vmsettings1.png)
    * Hardware
        * "Base memory" - Meg kell adnunk, hogy mennyi RAM-ot használjon fel. Érdemes a zöld vonalon belül maradni.
        * "Processors" - Meg kell adnunk, hogy hány magot kapjon a virtuális gép, szintén érdemes a zöld vonalon belül maradni.

    ![settings2](images/vmsettings2.png)

    * Hard Disk
        * Az utolsó beállítási menüpont a Hard Disk, itt három választási lehetőségünk van: 
            * Új virtuális Hard Disk létrehozása
            * Meglévő virtuális Hard Disk használata
            * Nem adunk hozzá virtuális Hard Disket
        * Esetünkben létrehozunk egy új Hard Disket. Meg kell adnunk, hogy hova hozza létre. Érdemes abba a mappába létrehozni, ahová telepíteni szeretnénk a virtuális gépet. 
        * Be kell állítanunk azt is, hogy mekkora tárhelyet kapjon a gép.
        * "Pre-allocate Full Size" - előre le lehet foglaltatni a tárhelymennyiséget amit megadtunk.
    * Ha ezekkel megvagyunk, kattinsunk a "Finish" gombra.

    ![settings3](images/vmsettings3.png)

## Virtuális gép futtatása 

1. Lemezkép csatolása
    * "Storage" menüpontnál kattintsunk az "[Optical Drive] Empty"-re, majd "Choose Disk Drive". Tallózzuk a lemezképet.
    ![optdrive](images/optdrive.png)

2. Gép futtatása
    * Kattintsunk a "Start" Gombra a gép futtatásához.
    ![new](images/new.png)

## Telepítés
1. Futtatás után fel és le nyilakkal irányítva, menjünk az "Install" gombra és nyomjunk Entert
![install](images/install.png)

2. Billentyűzet - nyilakkal vagy Tabbal navigálva keressük meg a Hungarian billentyűzetkiosztást és nyomjunk Entert
![keyboard](images/keyboard.png)

3. Particionálás - válasszuk ki a képek alapján
![partition](images/partition.png)
![partition2](images/partition2.png)
![partition3](images/partition3.png)
![partition4](images/partition4.png)
![partition5](images/partition5.png)

4. Várjuk meg a telepítést
5. Telepítsük a bootloadert
![bootloader](images/bootloader.png)
![bootloader2](images/bootloader2.png)
6. Continue
![complete](images/instcomplete.png)

## Ha befejeződött a telepítés, elindul a Raspberry Pi OS
### Telepítés
1. Nyomjunk "Next"-re
![rasp1](images/rasp1.png)

2. Válasszuk ki az országot és időzónát
![country](images/country.png)

3. Hozzunk létre felhasználót
![user](images/cruser.png)

4. Frissítsük a software-t
![software](images/updsoftware.png)

5. Állítsuk le a gépet
6. Vegyük ki a lemezmeghajtóból a lemezképet
7. **Indítsuk el a gépet, kész a telepítés**