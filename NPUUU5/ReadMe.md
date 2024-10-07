Tiny Core Linux

# Tiny Core Linux Telepítési Dokumentáció

## Bevezetés

A Tiny Core Linux egy minimalista Linux disztribúció, amelyet kis mérete és gyorsasága jellemez. Főként tapasztalt felhasználóknak és fejlesztőknek ajánlott, akik szeretnék testre szabni a rendszert.

## Rendszerkövetelmények

- **Processzor**: 32-bit vagy 64-bit támogatás
- **RAM**: Minimum 46 MB (64 MB ajánlott)
- **Tárhely**: Minimum 10 MB szabad hely
- **Boot eszköz**: USB, CD/DVD, vagy virtuális gép

## Telepítési lépések

### 1. ISO Kép Letöltése

1. Látogass el a (http://www.tinycorelinux.net).
2. Válaszd ki a megfelelő ISO képet (Core, TinyCore, vagy CorePlus) az igényeidnek megfelelően.
3. Töltsd le az ISO fájlt.

### 2. Bootolható Média Készítése

- **USB használata**:
  1. Használj programot, mint a Rufus (Windows), Etcher (Linux/Mac), vagy 'dd' (Linux) a bootolható USB készítéséhez.
  2. Válaszd ki a letöltött ISO fájlt és a cél USB meghajtót, majd indítsd el a folyamatot.

- **CD/DVD használata**:
  1. Írd ki az ISO képet egy CD/DVD-re a megfelelő író program segítségével.

### 3. Rendszer Indítása

1. Helyezd be a bootolható USB-t vagy CD/DVD-t a számítógépbe.
2. Indítsd újra a számítógépet, és állítsd be a BIOS/UEFI beállításokban a boot sorrendet úgy, hogy az USB/CD legyen az első.

### 4. Telepítési Opciók

1. A rendszer betöltése után választhatsz a következő opciók közül:
   - **Boot from CD/USB**: Alapértelmezett mód.
   - **Boot with no drive**: Minimalista indítás, csak a szükséges rendszerszolgáltatásokkal.

2. Válaszd ki a kívánt indítási módot, majd nyomj Enter-t.

### 5. Rendszerbeállítások

- A Tiny Core Linux alapértelmezés szerint a RAM-ba töltődik be, így bármilyen módosítás a következő indításkor elveszik.
- Használhatod a 'tc-install' parancsot a telepítéshez (a telepítés a merevlemezre történik).

### 6. Rendszer Telepítése a Merevlemezre

1. Nyisd meg a terminált, és futtasd a következő parancsot:
   ```bash
   sudo tc-install
   ```
2. Kövesd az utasításokat a telepítési folyamat során:
   - Válaszd ki a céleszközt (merevlemez).
   - Válaszd ki a partíciót, amelyre telepíteni szeretnéd.
   - Állítsd be a fájlrendszert (ext3/ext4 ajánlott).

### 7. Rendszerindítási Beállítások

- A telepítés befejezése után be kell állítanod a bootloader-t, mint például a GRUB vagy LILO, hogy a Tiny Core Linux elinduljon.

### 8. Rendszer Használata

- A Tiny Core Linux egy minimális rendszert biztosít, amelyhez további csomagokat lehet telepíteni a `tce-load` parancs segítségével.

