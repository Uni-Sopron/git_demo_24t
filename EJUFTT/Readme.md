<h1>Clear Linux telepítése</h1>
A Clear Linux telepítése a következő lépéseken keresztül történik:

<h2>1. Rendszerkövetelmények</h2>
Győződj meg róla, hogy a géped megfelel a Clear Linux minimális követelményeinek. Általában a következőkre van szükség:

-64 bites processzor<br>
-Legalább 1 GB RAM (ajánlott: 2 GB)<br>
-10 GB szabad lemezterület<br>

<h2>2. ISO letöltése</h2>
Látogass el a Clear Linux letöltési oldalára: https://cdn.download.clearlinux.org/releases/42100/clear/ és válaszd ki a clear-42100-live-server-t és töltsd le.
<h2>3. Virtuális gép létrehozása</h2>
VirtualBox megnyitása.
Kattints az „Új” gombra a virtuális gép létrehozásához.
Név: Adj nevet a virtuális gépnek (pl. "Clear Linux").
Típus: Válaszd az „Linux” lehetőséget.
Verzió: Válaszd az „Other Linux (64-bit)” lehetőséget.
RAM: Állíts be legalább 1 GB-ot (ajánlott 2 GB vagy több).
Virtuális merevlemez: Válaszd a „Virtuális merevlemez létrehozása” lehetőséget, majd kattints a „Létrehozás” gombra.
<h2>4. Virtuális merevlemez beállítása</h2>
Típus: Válaszd a „VDI (VirtualBox Disk Image)” lehetőséget.
Méretezés: Adj meg legalább 10 GB-ot a virtuális merevlemezhez.
<h2>5. ISO fájl csatolása</h2>
A létrehozott virtuális gép kiválasztása után kattints a „Beállítások” gombra.
A bal oldali menüben válaszd az „Adatlemezek” lehetőséget.
Kattints a „CD/DVD” ikonra, majd válaszd a „Válassz egy lemezképet” lehetőséget.
Navigálj a letöltött Clear Linux ISO fájlhoz, és válaszd ki.
<h2>6. Virtuális gép indítása</h2>
Kattints az „OK” gombra a beállítások mentéséhez.
A virtuális gép indításához kattints a „Start” gombra.
<h2>7. Telepítővarázsló</h2>
Amikor a Clear Linux boot menüje megjelenik, válaszd az „Install Clear Linux” opciót.
Kövesd a telepítővarázsló lépéseit:
Nyelv kiválasztása.
Telepítési típus (törlés vagy egyedi partíciók).
Felhasználói fiók beállítása.
Telepítés megkezdése.

<h2>8. Rendszerindítás</h2>
Miután a telepítés befejeződött, távolítsd el a CD/DVD meghajtót a virtuális gépből (a „Beállítások” > „Adatlemezek” menüben) és indítsd újra a virtuális gépet.
<h2>9. Első beállítások és frissítések</h2>
Az első indításkor bejelentkezés után futtasd a frissítéseket:
bash,sudo swupd update<br>.
Most már készen is állsz a Clear Linux használatára!



