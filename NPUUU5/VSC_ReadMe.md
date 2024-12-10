VSC telepítése Alpine Linuxra:

1. Készítsd elő az Alpine Linux rendszert
Először is győződj meg arról, hogy az Alpine Linux rendszer naprakész. Nyisd meg a terminált, és frissítsd a csomaglistát:
    sudo apk update
    sudo apk upgrade


2. Telepítsd a szükséges függőségeket
A Visual Studio Code telepítéséhez szükség van néhány csomagra, mint például a libx11, gtk, libxkbfile, stb. Telepítsd ezeket a következő parancsokkal:
    sudo apk add --no-cache libx11 libxkbfile libsecret gtk+3.0 \
    nss alsa-lib libcups libxcomposite libxrandr libxss libxtst \
    libdbus-glib libgcrypt


3. Telepítsd a Visual Studio Code-ot
Az Alpine Linux rendszer nem rendelkezik hivatalos Visual Studio Code csomagokkal, de használhatunk egy alternatív megoldást a Microsoft által karbantartott .deb csomagok telepítésével.

Először is töltsük le a legfrissebb .deb csomagot:
    wget https://update.code.visualstudio.com/latest/linux-deb-x64/stable -O code.deb
    
Most telepíthetjük a csomagot az dpkg eszközzel. Mivel az Alpine Linux nem támogatja közvetlenül az .deb csomagokat, szükség lesz a dpkg telepítésére:
    sudo apk add dpkg
    sudo dpkg -i code.deb

Ha hiányzik bármilyen függőség, akkor azt az apk segítségével telepítheted:
    sudo apk add --no-cache <hiányzó-függőség>

4. Indítsd el a Visual Studio Code-ot
Miután a telepítés befejeződött, indítsd el a Visual Studio Code-ot a következő parancsokkal:
    code

Vagy keresd meg a menüben és indítsd el az alkalmazást.

Grafikus telepítésről csatolok képeket.