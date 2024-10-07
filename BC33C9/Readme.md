## Előkészületek

1. **VirtualBox telepítése:**
   - Töltsd le és telepítsd az Oracle VirtualBoxot innen: [https://www.virtualbox.org/](https://www.virtualbox.org/).
   
2. **Edubuntu ISO letöltése:**
   - Látogasd meg az Edubuntu hivatalos weboldalát, és töltsd le a legújabb ISO fájlt: [https://www.edubuntu.org/](https://www.edubuntu.org/).

## 1. Virtuális gép létrehozása

1. Indítsd el a VirtualBoxot.
2. Kattints az **Új** (New) gombra a kezdőképernyőn.
3. Add meg a gép nevét (pl. "Edubuntu"), válaszd ki a **Típus**-nál a **Linux**-ot, és a **Verzió**-nál válaszd ki az **Ubuntu (64-bit)**-et.
4. Kattints a **Tovább** (Next) gombra.

## 2. Memória (RAM) beállítása

1. Állítsd be a RAM méretét. Javasolt legalább 2 GB (2048 MB), de minél több annál jobb, ha a rendszered engedi.
2. Kattints a **Tovább** gombra.

## 3. Virtuális merevlemez létrehozása

1. Válaszd ki a **Virtuális merevlemez létrehozása most** (Create a virtual hard disk now) opciót, majd kattints a **Létrehozás** (Create) gombra.
2. A következő ablakban válaszd a **VDI** (VirtualBox Disk Image) opciót.
3. A tárhely kiosztásnál válaszd a **Dinamikusan növekvő** (Dynamically allocated) lehetőséget, hogy a virtuális gép csak annyi helyet foglaljon, amennyit ténylegesen használ.
4. Állítsd be a lemez méretét legalább 20 GB-ra, majd kattints a **Létrehozás** gombra.

## 4. ISO fájl csatolása

1. A létrehozott virtuális gép kiválasztása után kattints a **Beállítások** (Settings) gombra.
2. A bal oldali menüben válaszd a **Tárolás** (Storage) opciót.
3. Kattints az **Üres** (Empty) CD ikonra, majd a jobb oldalon lévő CD ikonra kattintva válaszd a **Lemezkép kiválasztása** (Choose a disk file) opciót.
4. Töltsd be az Edubuntu ISO fájlt.

## 5. Virtuális gép elindítása

1. Kattints a **Start** gombra a VirtualBox főmenüjében.
2. Az Edubuntu telepítő elindul. Válaszd ki a **Try or Install Edubuntu** opciót.

## 6. Edubuntu telepítése

1. Válaszd ki a kívánt nyelvet (pl. Magyar), majd kattints a **Telepítés** (Install) gombra.
2. Kövesd az utasításokat: válaszd ki az időzónát, billentyűzetkiosztást és a partíciót.
   - A partíció beállításánál választhatod a **Lemez törlése és az Edubuntu telepítése** opciót, mivel ez egy virtuális gép.
3. Add meg a felhasználói fiók adatait (név, jelszó).
4. Kattints a **Telepítés most** gombra, és várd meg, míg a telepítés befejeződik.

Most már készen állsz az Edubuntu használatára a VirtualBox-ban!