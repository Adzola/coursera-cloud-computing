# coursera-cloud-computing
Repository for Coursera Cloud Computing Master

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

