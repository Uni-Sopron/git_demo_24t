# freeBSD útmutató a telepítéshez
#-------------------------------------------------------------------------#
1. Lépés: keresd fel a https://download.freebsd.org/ weboldalt
     ('Kepek/1.png')
2. Lépés: válaszd ki a számodra, pontosabban rendszerednek tetszőleges változatot 
(én az amd64-est valasztottam) --> majd töltsd le a FreeBSD-14.1-RELEASE-amd64-dvd1.iso.  nevű fájlt
('Kepek/2.png')
3. Lépés:  A c:\Users\felhasználóneved\VirtualBox Vms\ állományba létrehozol egy mappát amit elnevezel freeBSD-nek majd behúzod a letöWltött iso fájl-t mert így könnyebb lesz megtalálni a lemezképet.
#----------------------------------------------------------------------------#
       ! Konfigurálás virtualboxban:
            1. Hozz létre egy új virtuális gépet ezt megtudod tenni
              az "Új" nevű ikonra való kattintással tudod megtenni
              ('Kepek/5.png')
            2. Kiválasztod a létrehozott mappádat 
            ('Kepek/6.png')
            2.5 Kiválasztod az ún. ISO image-et/lemezképet: 
                *a fent említettek alapján tudod elérni a legegyszerűbben*
            ('Kepek/4.png')
            3. Tetszőlegesen beállítod a memóriaméretet a csúszka segítségével  --> beállítod a proci számot
            ('Kepek/8.png')
            4.Beállítod a virtuális merevlemez méretet (én úgy hagyom ahogy alapból van, 16GB) 
            ('Kepek/9.png')
             Miután megvagy, indítsd el a BSD-t.
:I------------------------------------------------------------------------------I:
    Free BSD installer - telepítő:
            ('Kepek/11.png')
         *nem kell  megijedni a terminálos megjelenítéstől végig ilyen lesz az op, rendszer ;D*

    #- az ENTER-rel és a  NYILAKKAL tudsz navigálni a menüsorokban -#
        1. Válaszd ki az "INSTALL" opciót és nyomj egy ENTERT
        2. Válaszd ki a billenytyűzeted régiódnak/származásodnak megfelelően
        ('Kepek/12.png')
        3. Írj egy tetszőleges hostnevet pl: lajosPC vagy heckerjani
        ('Kepek/13.png')
        4. Menj rá a legelső opcióra a "BASE SYSTEM DEBUGGING"-ra
              ('Kepek/14.png')
        5.  Majd szintén a legelső opcióra "AUTO ZFS - GUIDED ROOT-ON-ZFS "-re 
           a következőt fogja kiiírni "PROBING DEVICES PLEASE WAIT"
           
        6. CONFIGURE OPTIONS --> ">>INSTALL Proceed with installation" 
          ('Kepek/15.png')
         -->" STRIPE-
        NO REDUNDANCY" --# ezt követően ki fog adni egy "[] ada0 VBOX HARDDISK" -et
        melyet a SPACE gomb megnyomásával tudod abszolválni majd ütsz egy ENTERT.
         ('Kepek/16.png')
       7. Megfogja kérdezni hogy biztosan TÖRÖLNI akarjuk-e a lemez tartalmát?
            Nyugodtan üssünk a "YES" opcióra.
            ('Kepek/17.png')
        8. Kérni fog tölünk egy új jelszót és annak megismétlését mindegyik megadása után üssünk egy ENTERT.
        ('Kepek/19.png')
        9. Kérni fogja az időzónát természetesen szintén személyes preferenciának
        megfelelően tegyük ezt meg.  Meg is  kérdezi a rendszer hogy megfelelőnek tűnik-e automatikusan beállított idő amennyiben nem, annak módosítását tegyük meg.
        ('Kepek/22.png')
        10. Válasszuk ki azt szolgáltatást amit szeretnénk hogy boot-kor indítson a rendszer:
            ('Kepek/23.png') ('Kepek/24.png')
            "Local caching validation resolver"-t válasszuk ki
            majd szintén az első opcióra ("HIDE UID")-ra menjünk
        11. Megkérdezi a rendszer hogy óhajtunk-e hozzáadni felhasználokat ?
          ('Kepek/26.png')
             Természetesen igen, hiszen önmagunkat hozzá kell adnunk.
        Adjuk meg a Felhasználónevünket ('Kepek/26.png')  
        majd minden kérdésre üssünk egy ENTERT  míg a jelszavunkat nem kéri ha szeretnénk jelszóval védeni fiókunkat.
        ('Kepek/27.png')
        Végső soron megmutatja az általad megadott paramétereket és megkérdezi hogy "OK?" amennyiben minden megfelel akkor írjunk egy "YES"-t
        illetve azt is hogy hozzá akarunk-e adni egy másik felhasználót:
         A válasz opciónális.
         / Amennyiben igen, akkor ismételjük meg az utóbb említett lépéseket a felhasználónév és  a jelszó megadásának módjának kivételével   /
        12.  A SETUP végénél : válasszuk az "APPLY CONFIGURATION AND EXIT INSTALLER" opciót. Majd felajánlja a végső módosítás lehetőségét.
        ('Kepek/28.png')('Kepek/29.png')
        13. Amennyiben nem volt szükséges a módosítás, visszadob a kezdő menüpontba
        és válasszuk a "REBOOT-ot".
        
        Ezt követően kapcsoljuk ki a virtulis gépet és csatoljuk le az iso-fájlt az optikai meghajtóról (konfigurálás--> tároló--> ...iso fájl leválasztása)
---------------------------------------------------------------------------------- 

 Első lépések:
     Indítsuk újra a gépünket majd válasszuk a boot menüpontból a "multi user boot"
     opciót a 1-es gomb megnyomásával.
     kérni fogja tőlünk a login-t (felhasználóneved) és a jelszavad

Ha sikeresen megadtad belépési adataid akkor:
('Kepek/30.png')
    felhasznaloneved@hostneved: -nak kell látszódnia
#--------------------------------------------------------------------------------#    
               ,        ,         
               /(        )`        
               \ \___   / |        
               /- _  `-/  '        
              (/\/ \ \   /\        
              / /   | `    \       
              O O   ) /    |       
              `-^--'`<     '       
             (_.)  _  )   /        
              `.___/`    /         
                `-----' /          
   <----.     __ / __   \          
   <----|====O)))==) \) /====|      
   <----'    `--' `.__,' \         
                |        |         
                 \       /       /\
            ______( (_  / \______/ 
          ,'  ,-----'   |          
          `--{__________)          

          Gratulálok sikeresen telepítetted az Op.rendszered ! Jó szórakozást kívánok ! :D