# EndeavourOS telepítési útmutató

## VirtualBox beállítások

![Kezdő oldal VirtualBox](virtualbox_kezdolap.png)
A **New** gombra kattintva tudunk egy új virtuális gépet létrehozni!

![Alap beállítások VirtualBox](virtualbox1.png)
Először a **Name and Operating System** kategórán belül végezzük el a szükséges beállításokat! A *Name* részben adunk nevet a virtuális gépünknek, ami bármi lehet, nincsenek karakter hossz vagy speciális karakter megkötések! A *Folder* részt hagyhatjuk ahogy van! Az *ISO Image* részben kiválasztjuk az [Endeavour oldaláról](https://endeavouros.com/) letöltött ISO fájlt. A *Type* részben a **Linux** operációs rendszert válasszuk ki, majd a többi kategórát úgy hagyjuk!

![Hardware kategória VirtualBox](virtualbox2.png)
A **Base Memory** részben adjuk meg a RAM-ot a virtuális gépünknek, ami a példában 4096 MB vagyis 4GB, ami tökéletesen elég lesz. Alatta a *Processors* részben adjuk meg a CPU magok számát, ami a példán 2 db.

![Hard Disk kategória VirtualBox](virtualbox3.png)
A **Hard Disk** kategórián belül amin változtatunk az a *Create a Virtual Hard Disk Now* részen van, ahol beállíthatjuk a virtuális gép merevlemezének helyét és méretét. Ha ezekkel megvagyunk, akkor kattintsunk lent a **Finish** gombra!

![Settings VirtualBox](virtualbox_kezdolap.png)
Ezután a **Settings** gombra kattintva további beállításokat fogunk végezni!

![System kategória VirtualBox](virtualbox_beallitasok1.png)
A **System** kategóriában először is a kékkel karikázott részt nézzük át, itt ugyanis az OP rendszer boot-olási sorrendje van feltüntetve. A *Floppy* van az első helyen, ami nem lesz jó, mert már ilyet nem használunk, szóval innen nem fog tudni beboot-olni a rendszer, ezért pipáljuk ki, majd húzzuk le a sor legaljára!

![Display kategória VirtualBox](virtualbox_beallitasok2.png)
Ha átkattintottunk a **Display** kategóriára, akkor a *Video Memory* részen található csúszkát húzzuk fel maximumra és minden mást hagyjunk meg eredeti állapotában!

![Storage kategória VirtualBox](virtualbox_beallitasok3.png)
A **Storage** kategóriában kattintsunk rá az ISO fájlra, majd pedig pipáljuk be a *Live CD/DVD* opciót, amit a kék karika jelez!

Ezek után kattintjunk az **OK** gombra, majd pedig fent középen a **Start** gombra, ls el is indíthatjuk az OP rendszerünket!

![Endeavour indítás](endeavour_inditas.png)
A képen látható lehetőség kiválasztása után nyomjon egy *Enter*-t!

![Endeavour telepítője](endeavour_telepito.png)
Miután elindult az OP rendszer, felugrik a telepítő! Itt válassza ki a *Start the Installer* lehetőséget!

![Endeavour telepítő metódus](endeavour_telepito_metodus.png)
Itt válassza az **Offline** opciót!

![Endeavour nyelv](endeavour_nyelv_valasztas.png)
Itt válassza ki a nyelvet!

![Endeavour régió](endeavour_regio_valasztas.png)
Itt válassza ki a régiót!

![Endeavour billentyűzet](endeavour_billentyuzet_valasztas.png)
Itt válassza ki a billentyűzetet!

![Endeavour GRUB](endeavour_GRUB.png)
Itt válassza ki a **GRUB** lehetőséget!

![Endeavour particionálás](endeavour_particiok.png)
Itt válassza ki a **Manuális particionálás** lehetőséget!

![Endeavour MBR](endeavour_MBR.png)
Itt válassza ki a **Master Boot Record** lehetőséget!

![Endeavour root](endeavour_root.png)
A **Létrehozás** gombra való kattintás után először adja meg a gyökér könyvtár méretét, ami az én esetemben 25 GB! Csatolási pontnak a **/** opciót válassza, majd **Jelölők** részben a *root* opciót válassza!

![Endeavour swap](endeavour_swap.png)
A **Létrehozás** gombra való kattintás után először adja meg a swap méretét, ami az én esetemben 4 GB! A **Jelölők** részben a *swap* opciót válassza, a **Fájlrendszer** kategóriában pedig a *linuxswap* opciót!

![Endeavour felhasználó létrehozása](endeavour_felhasznalo.png)
Itt töltse ki a megadott mezőket!

Ezek után kattintson a telepítés gombra, majd pedig várjon, amig elkészül a telepítés. Ezek után indítsa újra a rendszert!

![ISO fájl lecsatolása](ISO_fajl_lecsatolas.png)
Miután a rendszert bezárta, ismét menjen a **Storage** kategóriába a VirtualBox-on belül, és kattintson jobb egérgombbal az ISO fájlra, ahol megjelenik a *Remove Attachment* gomb. Kattintson rá, és csatolja le az ISO fájlt!

Ezek után bármikor el tudja indítani a virtuális gépet!