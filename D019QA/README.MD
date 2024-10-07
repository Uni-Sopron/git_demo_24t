# Az Arch  Linux telepítési útmutatója
### Teendők live imageben
A live image angol billentyűzetkiosztással indul, a magyarhoz írjuk be a ***loadkeys hu*** parancsot.
Én kábeles netet használtam, így néhány lépéssel megkönnyítettem a dolgomat, wifis csatlakozás esetén azonban az alábbi parancsokat kéne követni: 
1. iwctl
2. device list
3. station wlan0 scan
4. station wlan0 get-networks
5. station wlan0 connection *hálózatnév*
    > Passphrase - wifi jelszó beírása
6. station wlan0 show - azt kell látnunk, hogy *connected*
7. exit

Ha ezzel elkészültünk, az ***archinstall*** parancs következik. A parancs beírása után egy ablak jelenik meg előttünk sok beállítható lehetőséggel.

Én a következő beállításokat végeztem el:

| Menüpont   | Kiválasztandó opció  | Azon belül 1      | A.b. 2 |
| :-------:  | :------------------- | -----------------:| :-----:|
| Mirrors    | Mirror region        | Hungary            | |
| Locales    | Keyboard layout      | hu                | |
|            | Locale language      | hu_HU.UTF8        | |
|            | Locale encoding      | UTF-8             | |
| Disc conf. | Manual Partitioning  | Loopback deviced  | ext4 |
| Bootloader | Grub                 |                   | |
| Swap       | True                 | | |
| Hostname   | [a számítógéphez tartozó hostname megadása] | | |
| Root passw.| [a rendszergazda jelszavának megadása]      | | |
| User acc.  | [a számítógéphez tartozó felhasználók megadása]| Confird and exit | |
| Profile    | Desktop             | Cinnamon | |
| Audio      | Pulseaudio          | | |
| Kernels    | linux-zen           | | |
| Net. conf. | Use Network Manager | | |
| Timezone   | Europe/Budapest     | | |
| NTP        | True                | | |
| Optional r.| multilab            | | |
| Install    |||
>Ha a telepítés után nem kívánunk további beállításokat végrehajtani, válasszuk a ***no*** opciót, és indítsuk újra a gépet a ***reboot*** paranccsal. 😉

Ezek után szükségünk lesz még a <mark> ***pacman csomagkezelőre*** </mark> , a terminálba beírandó parancsok: 
- sudo pacman -Syu 
- sudo pacman -S *csomagnév*
>Az interneten keresgélhetünk, miket lehet a *csomagnév* helyére beírni, innentől kezdve ez csak rajtunk múlik.

Az Arch Linux telepítéséhez segítségül vettem az alábbi YouTube videót:
https://www.youtube.com/watch?v=flI1njGcBuU


