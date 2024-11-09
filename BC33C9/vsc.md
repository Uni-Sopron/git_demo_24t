# Visual Studio Code Telepítése Edubuntura

1. **Frissítsd a csomagokat**: Nyiss egy terminált és futtasd az alábbi parancsot: `sudo apt update`

2. **Csomagok telepítése**: Telepítsd a szükséges csomagokat a következő paranccsal: `sudo apt install software-properties-common apt-transport-https wget`

3. **Microsoft GPG kulcs és repository hozzáadása**: Töltsd le a Microsoft GPG kulcsot és add hozzá a repository-t: `wget -qO- https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -` majd `sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"`

4. **Visual Studio Code telepítése**: Frissítsd újra a csomagokat, majd telepítsd a Visual Studio Code-ot: `sudo apt update` majd `sudo apt install code`

5. **Indítás**: A telepítés után indítsd el a Visual Studio Code-ot az alábbi paranccsal: `code`

![VSCode ikon](visualstudio_code_logo.png)