# coursera-cloud-computing
Repository for Coursera Cloud Computing Master

**********************************************************************************************************************************************************
Powershell ISE 

#Enable-WindowsOptionalFeature -Online -FeatureName "Microsoft-HypervisorPlatform" -All
#Get-WindowsOptionalFeature -Online -FeatureName "Microsoft-HypervisorPlatform"
#DISM /Online /Enable-Feature /FeatureName:Microsoft-Hyper-V-All /All



winget install powershell --source=winget

winget install git.git --source=winget

winget install vagrant --source=winget

winget search "Windows Terminal" --accept-source-agreements 

winget install "Windows Terminal" --source=msstore    #sajnos ezt konzolbol kell futtatni vagy így:

winget install "Windows Terminal" --source=msstore --accept-source-agreements --accept-package-agreements

winget install "Microsoft Visual Studio Code" --source=msstore #sajnos ezt konzolbol kell futtatni, vagy így:

winget install "Visual Studio Code" --source=msstore --accept-source-agreements --accept-package-agreements


winget install virtualbox --source=winget

winget install virtualbox vagrant packer

#ssh-keygen -t ed25519   #Ez se fut le így

*****************************************************************************************************************************************************************
public/private key pair
ssh-keygen -t ed25519

Claude Haiku 3.5
Az ssh-keygen -t ed25519 parancs egy új SSH kulcspárt hoz létre az Ed25519 algoritmus használatával. Nézzük részletesen:

Kulcstípus: Ed25519
Modern, biztonságos nyilvános kulcsú aláíró algoritmus
Kompakt és gyors
Erős kriptográfiai biztonságot nyújt
Folyamat:
Létrehoz egy privát kulcsot
Létrehoz egy hozzá tartozó nyilvános kulcsot
Alapértelmezetten a ~/.ssh/ könyvtárba menti a kulcsokat
Lehetőséget ad jelszó beállítására a privát kulcshoz
Alapvető opciók:
-t ed25519: Ed25519 kulcstípus kiválasztása
Rákérdez a mentési helyre
Opcionálisan jelszót kérhet
Felhasználási módok:
Biztonságos SSH bejelentkezés
Git repository hitelesítés
Szerver és távoli gépek biztonságos elérése
**************************************************************************************************************************************************************************
Úgy tünik hogy ha clone-ni akarom akkor jelszót kér.
A terminálba a parancs!
git clone git@github.com:Adzola/coursera-cloud-computing.git

**************************************************************************************************************************************************************************
Copilot:
Nagyszerű kérdés, Zoltán! Ha ezt a Git tárolót szeretnéd klónozni a terminálból, és az SSH kulcsod már be van állítva a GitHub-fiókodhoz, akkor a parancs a következő:

bash
git clone git@github.com:Adzola/coursera-cloud-computing.git
✅ Fontos előfeltételek:
SSH kulcs legyen generálva és hozzáadva a GitHub-fiókodhoz. Ellenőrizheted a ~/.ssh/id_rsa.pub vagy ~/.ssh/id_ed25519.pub fájlokat.

Git legyen telepítve a rendszereden. Ellenőrizheted ezzel:

bash
git --version
🔍 Ha hibát kapsz:
Ha „Permission denied (publickey)” hiba jön, akkor az SSH kulcs nincs megfelelően konfigurálva.

Ebben az esetben vagy használhatod a HTTPS verziót:

bash
git clone https://github.com/Adzola/coursera-cloud-computing.git
…vagy beállítjuk az SSH kulcsot, ha ragaszkodsz az SSH-hoz.

**************************************************************************************************************************************************************************
milyen parancs-csal tudom visszatölteni a gitubra?
Remek kérdés! Ha módosítottál fájlokat a klónozott projektben, és szeretnéd visszatölteni (push-olni) őket a GitHubra, akkor az alábbi lépések és parancsok segítenek. Feltételezem, hogy már klónoztad a repót SSH-n keresztül, és van jogosultságod írni rá.

🚀 Git visszatöltés lépésről lépésre
1. Fájlok hozzáadása a staging area-hoz
bash
git add .
Ez minden módosított és új fájlt hozzáad a commithoz. Ha csak egy konkrét fájlt akarsz:

bash
git add path/to/file.txt
2. Commit létrehozása
bash
git commit -m "Rövid, de értelmes üzenet a változásról"
Például:

bash
git commit -m "Frissítettem a README-t és hozzáadtam a scriptet"
3. Push a GitHubra
bash
git push origin main
🔁 Ha az ág neve nem main, hanem például master vagy más, akkor azt kell használnod:

bash
git push origin master
🧠 Ellenőrzés
Ha nem vagy biztos az aktuális ág nevében:

bash
git branch
Ha nem tudod, milyen távoli repó van beállítva:

bash
git remote -v
💡 Tipp
Ha ez az első push, és még nincs upstream beállítva:

bash
git push --set-upstream origin main

********************************************************************************************************************************************************************




