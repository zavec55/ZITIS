# ZITIS

## Dokumentacija za vzpostavitev projekta

### 1. Sistemske zahteve

- **Operacijski sistem**: Windows
- **IDE**: Visual Studio Code (priporočljivo, ker je bilo testirano in potrjeno, da deluje ustrezno)
- **Framework**: Express (Node.js)
- **Baza podatkov**: MongoDB (lokalno ali oddaljeno)
- **Spletni brskalnik**: Google Chrome, Firefox ali drugi

### 1.1 Koraki namestitve

#### 1.2 Namestitev Node.js in Express:
1. Obiščite [Node.js uradno spletno stran](https://nodejs.org/) in prenesite namestitveno datoteko za Windows.
2. Namestite Node.js, ki bo vključeval tudi npm (Node Package Manager).
3. Po namestitvi Node.js odprite ukazno vrstico (Command Prompt) v Visual Studio Code in preverite namestitev z naslednjimi ukazi:
    ```bash
    node -v
    npm -v
    ```
4. Namestite Express globalno z naslednjim ukazom:
    ```bash
    npm install -g express
    ```

#### 1.3 Namestitev in Konfiguracija MongoDB:
1. Prenesite MongoDB iz [uradne strani MongoDB](https://www.mongodb.com/try/download/community) in ga namestite lokalno, ali pa uporabite obstoječo oddaljeno bazo.

#### 1.4 Prenos in Namestitev YogaFlex:
1. Prenesite projektno mapo YogaFlex iz uradnega repozitorija ali vira.
2. Razpakirajte projektno mapo na želeno lokacijo na računalniku (npr. `C:\Projects\YogaFlex`).

#### 1.5 Konfiguracija Visual Studio Code:
1. Odprite Visual Studio Code.
2. Izberite **File > Open Folder** in izberite mapo z aplikacijo YogaFlex.
3. Prepričajte se, da imate nameščene vtičnike za delo z Node.js in Express (npr. ESLint, Node.js Extension Pack).

#### 1.6 Nastavitev in Povezava z MongoDB bazo:
1. Aplikacija YogaFlex je privzeto nastavljena za povezavo z obstoječo MongoDB bazo.
2. V datoteki `server.js` lahko spremenite dostop do svoje podatkovne baze.
3. Če želite uporabiti svojo MongoDB bazo, spremenite `mongoose.connect` v ustrezno povezavo (URI) do vaše baze.
   > **Opomba**: V primeru spremembe URI-ja bo potrebno ročno vnesti podatke v bazo, saj privzeta baza vsebuje že nastavljene podatke za uporabo aplikacije.

#### 1.7 Nastavitev in Zagon Localhost Strežnika:
1. V ukazni vrstici Visual Studio Code zaženite:
    ```bash
    npm install
    ```
    To bo namestilo vse potrebne odvisnosti, ki jih zahteva aplikacija YogaFlex.
2. Po namestitvi odvisnosti, zaženite aplikacijo z naslednjim ukazom:
    ```bash
    npm start
    ```
    ali z ukazom:
    ```bash
    node server.js
    ```
3. Aplikacija bo sedaj na voljo na `localhost:3000`. Odprite brskalnik in obiščite:
    ```
    http://localhost:3000/home.html
    ```

### 1.8 Opomba
Čeprav lahko aplikacijo YogaFlex razvijate in zaženete v kateremkoli IDE-ju ali urejevalniku besedil, priporočamo uporabo Visual Studio Code, saj je bilo to okolje že predhodno testirano in je potrjeno, da deluje brez težav.
