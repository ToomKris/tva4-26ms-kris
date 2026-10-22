# 💻 Kooli projektid

👋 Olen **Tallinna Tehnoloogiakolledži (TTK / Techno TLN)** õpilane ja siin repos on minu tööd aines **Rakendus serverite alused**.

🛠️ Projektid on loodud vibekodeerimise ja Claude’i abil. Nende eesmärk on anda praktiline ülevaade sellest, kuidas toimivad koodi pull’imine, projektide haldamine ja arendusega seotud töövood. Ühtlasi tutvustavad need agiilse tarkvaraarenduse esimesi samme ning aitavad mõista, kuidas ideest jõutakse toimiva lahenduseni.

## 🌐 Portfolio

* **Portfolio:** https://toomkris.github.io/work

## 📝 Kodutöö 1 – vastused

**Mis vahe on veebiserveril ja rakendusserveril?**
Veebiserver (nt nginx) võtab vastu HTTP-päringuid ja saadab tagasi valmis faile: HTML, CSS, pildid. Ta ei arvuta midagi, vaid annab kettalt olemasoleva faili. Rakendusserver (nt Node.js `server.js`) käivitab koodi ja loob vastuse iga päringu jaoks eraldi: loeb andmebaasi, töötleb andmeid ja tagastab näiteks JSON-i (`/api/notes`). Tavaliselt on veebiserver ees ja suunab API-päringud rakendusserverile edasi (*reverse proxy*).

**Mis on 404 ja 502 erinevus?**
- **404 Not Found:** server töötab, aga küsitud aadressil pole midagi (vale URL või fail puudub). Viga on päringus.
- **502 Bad Gateway:** veebiserver (proxy) töötab, aga ei saa tema taga olevalt rakendusserverilt korralikku vastust, näiteks seetõttu, et rakendus on maas või jooksis kokku. Viga on serveri poolel.
