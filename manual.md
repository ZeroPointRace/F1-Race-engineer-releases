# F1 Race Engineer — Felhasználói Kézikönyv

> **Játék:** EA Sports F1 25 (alap + 2026 Season Pack DLC) · **Verzió:** lásd a főmenü bal alsó sarkában
> **Támogatás:** f1zeropointracing@gmail.com

---

## Tartalomjegyzék

1. [Telepítés](#1-telepítés)
2. [Első indítás és licenc](#2-első-indítás-és-licenc)
3. [Licenckulcs beírása](#3-licenckulcs-beírása)
4. [F1 25 beállítása](#4-f1-25-beállítása)
5. [Verseny közbeni használat](#5-verseny-közbeni-használat)
6. [Hibaelhárítás](#6-hibaelhárítás)

---

## 1. Telepítés

### Rendszerkövetelmények

| Komponens | Minimum |
|---|---|
| Operációs rendszer | Windows 10 64-bit (vagy újabb) |
| RAM | 4 GB |
| Processzor | Bármely 2015 utáni x64 CPU |
| Hálózat | Internetkapcsolat (licenc-aktiváláshoz és első indításhoz) |
| Játék | EA Sports F1 25 (PC) |

### A telepítő letöltése

A telepítő **mindig a legfrissebb verzióval** itt érhető el:

👉 **https://github.com/ZeroPointRace/F1-Race-engineer-releases/releases/latest**

1. Nyisd meg a fenti linket
2. Az **„Assets"** szekcióban kattints a `F1-Race-Engineer-Setup-x.y.z.exe` fájlra
3. Ha a böngésző „nem biztonságos" figyelmeztetést ad, kattints a **Mentés** / **Megtartás** gombra — a fájl biztonságos, csak nincs (fizetős) kód-aláírási tanúsítvány

### Telepítés

A telepítő **egykattintásos**: nincs varázsló, nincs mappa-választás.

1. Futtasd a letöltött `.exe`-t
2. Ha Windows SmartScreen-figyelmeztetés jelenik meg → **„További információ"** → **„Futtatás mindenképpen"**
3. A program **automatikusan feltelepül és elindul** (a felhasználói mappádba, rendszergazda jog nélkül), és létrehoz egy asztali + Start menü parancsikont **„F1 Race Engineer"** néven

> 💡 Az **első** telepítéshez kell csak a fenti link. Onnantól a program **automatikusan frissül** (lásd a 6. fejezetet) — a következő verziókat magától letölti és felajánlja.

---

## 2. Első indítás és licenc

### Az alkalmazás elindítása

Kattints duplán az **F1 Race Engineer** asztali parancsikonra. Megjelenik a bevezető splash képernyő, majd az alkalmazás főmenüje.

> A háttérben automatikusan elindul a motor (backend), ez néhány másodpercet vesz igénybe első alkalommal. Ne zárd be az ablakot amíg betölt.

### Trial (ingyenes próbaidőszak)

Ha még nincs fizetős licenckulcsod, az alkalmazás automatikusan **14 napos próbaidőszakot** indít. Ezt nem kell aktiválni, azonnal működik.

A próbaidőszak alatt minden funkció elérhető, a főmenüben látható, hány nap maradt.

**A trial lejárta után** az alkalmazás korlátozva fut (csak a beállítás-oldalak érhetők el), versenytámogatás nincs — ekkor licenckulcsot kell bevinni.

---

## 3. Licenckulcs beírása

### Kulcs megszerzése

Licenckulcsot a fejlesztőtől szerezhetsz (email: f1zeropointracing@gmail.com). A kulcs formátuma: `XXXXX-XXXXX-XXXXX-XXXXX`.

### Aktiválás lépései

1. Nyisd meg az alkalmazást
2. A főmenüben kattints a **"Licenc"** gombra
3. Írd be a kulcsot a megfelelő mezőbe (kötőjelekkel vagy anélkül, mindegy)
4. Kattints az **"Aktiválás"** gombra
5. Ha az internetkapcsolat él és a kulcs érvényes → **"Licenc aktiválva"** üzenet jelenik meg

> Az aktiválás az adott géphez köti a kulcsot (hardver-azonosítón alapul). Ha új gépre kell átvinni, keress minket emailben.

### Mit mutat a licenc-oldal?

| Állapot | Jelentés |
|---|---|
| ✅ Aktív | Minden funkció elérhető |
| ⏳ Trial (N nap maradt) | Próbaidőszak, összes funkció elérhető |
| ❌ Lejárt | Trial vagy licenc lejárt — kulcs beírása kell |
| 🔒 Visszavont | A kulcsot érvénytelenítettük (pl. visszaélés esetén) |
| 📡 Offline | Nincs net, de a 7 napos grace-period él — minden megy |

---

## 4. F1 25 beállítása

Az F1 Race Engineer a játék UDP telemetria-adatfolyamát hallgatja. Ezt egyszer kell beállítani.

### Telemetria bekapcsolása F1 25-ben

1. Indítsd el az F1 25-öt
2. Menj: **Settings → Telemetry Settings**
3. Állítsd be az alábbi értékeket:

| Beállítás | Érték |
|---|---|
| UDP Telemetry | **On** |
| UDP IP Address | `127.0.0.1` (ha ugyanazon a gépen játszol) |
| UDP Port | **20777** |
| UDP Send Rate | **20Hz** vagy **60Hz** |
| UDP Format | **2025** (alap) vagy **2026** (2026 Season Pack DLC esetén) |
| Your Telemetry | **Public** |

> 💡 Ha konzolról streamed a játékot PC-re (Remote Play), az IP-cím nem `127.0.0.1`, hanem a konzol hálózati IP-je. Ebben az esetben keress minket.

### Az alkalmazás beállítása

1. A főmenüben kattints a **"Verseny beállítások"** gombra
2. Állítsd be:
   - **Pályahossz:** az aktuális futam pályája (vagy hagyd automatikusan)
   - **Stratégia módja:** Auto (ajánlott) vagy Manual
   - **Hang:** hangerő és hang be/ki
   - **Nyelv:** Magyar vagy English
3. Kattints a **"Beállítások mentése"** gombra — visszakerülsz a főmenübe

> A beállítások a gépeden tárolódnak, következő indításkor nem kell újra megadni.

---

## 5. Verseny közbeni használat

### Az alkalmazás elindítása verseny előtt

1. Indítsd el az **F1 Race Engineer**-t
2. Indítsd el az **F1 25**-öt (sorrendje mindegy, de érdemes az F1 RE-t előbb)
3. Menj be a versenymenübe — az alkalmazás automatikusan felismeri a sessiont és a megfelelő nézetbe vált

### A főmenü gombjai

| Gomb | Funkció |
|---|---|
| **Verseny** | Megnyitja az élő dashboard-ot |
| **Verseny beállítások** | Stratégia és hang beállítása |
| **Nyelv** | Magyar / English váltás |
| **Licenc** | Licenckulcs kezelése |

### A Dashboard (élő verseny nézet)

A Dashboard automatikusan megnyílik, amikor az F1 25 futamot érzékel. Mutatja:
- **Pozíció** és rés az előtted / mögötted lévőhöz
- **Gumiállapot** (kopás %, hőmérséklet — kék=hideg, zöld=optimális, piros=túlforró)
- **ERS szint** és használat
- **Szél- és időjárás-előrejelzés**
- **SC/VSC státusz** (Safety Car aktív esetén sárga sáv)
- **Döntési javaslatok** — amit a mérnök mond, az itt is megjelenik szövegként

### A mérnök hangutasításai — mit jelent, amit mond?

Az alkalmazás **magyarul** (vagy angolul, beállítástól függően) szól hozzád verseny közben. Íme a legfontosabb üzenetek:

**Gumikezeléssel kapcsolatos:**
| Üzenet | Jelentés |
|---|---|
| *"Gumik hidegek..."* | A gumihoz még nincs elég hő, óvatosan a kanyarokban |
| *"Gumik optimális hőmérsékleten"* | Most a legjobb a tapadás |
| *"Gumik túlmelegedtek!"* | Csökkentsd a tempót, hűtsd a gumikat |
| *"Kritikus gumiállapot!"* | Azonnali kiállás szükséges lehet |

**Boxstratégiával kapcsolatos:**
| Üzenet | Jelentés |
|---|---|
| *"Közelít a pit-ablak"* | 3-5 körön belül érdemes kiállni |
| *"Állj ki most!"* | Optimális pillanat a kiállásra |
| *"SC alatt olcsó kiállás"* | Safety Car aktív — most érdemes kiállni, kisebb időveszteség |
| *"Kötelező gumiváltás van"* | Még ki kell állnod a verseny végéig |

**Taktikával kapcsolatos:**
| Üzenet | Jelentés |
|---|---|
| *"Undercut veszély!"* | Az előtted lévő hamarosan kiállhat, előzd meg |
| *"Dirty air csapda"* | Túl sokáig vagy az előtted lévő mögött, az gumidat rongálja |
| *"Védekezési pozíció"* | A mögötted lévő közel van, figyeld a belső íveket |

**Időjárással kapcsolatos:**
| Üzenet | Jelentés |
|---|---|
| *"Eső közeledik"* | Néhány körön belül változik az időjárás |
| *"Rossz gumin vagy az esőhöz!"* | Azonnal válts esőgumira |
| *"Pálya szárad"* | Hamarosan vissza lehet váltani slick-re |

**Biztonsági autó / zászlók:**
| Üzenet | Jelentés |
|---|---|
| *"Safety Car kiküldve!"* | Lassíts, kövesd a biztonsági autót |
| *"Virtuális Safety Car"* | VSC aktív — lassíts a delta szerint |
| *"Safety Car visszavonul"* | Hamarosan újraindul a verseny, készülj |
| *"Kék zászló!"* | Engedd el az előtted lévő vezető kört autót |
| *"Időbüntetést kaptál!"* | Büntetés érkezett, a mérnök megmondja mennyi |

### Élő pályatérkép

A Dashboard jobb felső sarkában a 🗺️ **Térkép** gombra kattintva külön ablakban megnyílik az élő pályatérkép:
- Minden autó valós időben látható
- Saját autód sárga kiemelővel jelölt
- Gumiösszetétel, rés-adatok, sárga zónák jelölve
- SC/VSC esetén sárga banner pulzál a térkép tetején

---

## 6. Hibaelhárítás

### "Nem csatlakozik" / A Dashboard üres

**Lehetséges okok és megoldások:**

1. **Az F1 25 UDP telemetria ki van kapcsolva**
   → Menj az F1 25 beállításaiba, és ellenőrizd (lásd [4. fejezet](#4-f1-25-beállítása))

2. **Rossz IP-cím az F1 25-ben**
   → Ha ugyanazon a gépen játszol, az UDP IP legyen `127.0.0.1`

3. **Tűzfal blokkolja a 20777-es portot**
   → Windows Defender Firewall → Engedélyezett alkalmazások → adj engedélyt az F1 Race Engineer-nek

4. **Az alkalmazás nem töltött be teljesen**
   → Zárd be és nyisd meg újra, várj 10 másodpercet a splash képernyő után

---

### A mérnök nem szól semmit

1. **Verseny session-ben vagy-e?** A mérnök csak futam közben szól (kvalifikáció és edzés alatt néma)
2. **Hangerő be van-e kapcsolva?** Ellenőrizd a Verseny beállításokban
3. **Windows hangbeállítás** → Győződj meg róla, hogy az alkalmazás nincs némítva (tálca jobb klikk → Hangerő-beállítás)
4. **Első pár kör** → Az alkalmazásnak néhány köre kell, mire elég adat gyűlik a tanácsokhoz

---

### "Lejárt trial" / "Érvénytelen licenc" üzenet

- Ha a 14 napos trial lejárt → licenckulcsot kell bevinni ([3. fejezet](#3-licenckulcs-beírása))
- Ha elvesztetted a kulcsodat → írj emailt: f1zeropointracing@gmail.com

---

### "Háttérrendszer timeout" indításkor

Az alkalmazás nem tudta elindítani a belső motort 30 másodperc alatt.

**Megoldás:**
1. Zárd be az alkalmazást teljesen
2. Várj 5 másodpercet
3. Nyisd meg újra
4. Ha ismétlődik: telepítsd újra az alkalmazást (a beállításaid megmaradnak)

---

### Frissítések (automatikus)

Az F1 Race Engineer **automatikusan frissül** — nincs szükség kézi letöltésre. Amikor új verzió jelenik meg:

1. Indítás után a főmenüben megjelenik egy **frissítés-sáv**: *„🔄 Új verzió elérhető… ⬇ letöltés %… ✅ kész"*
2. A sávban látod az **újdonságokat** is (mi változott ebben a verzióban).
3. Kattints az **„Újraindítás most"**-ra → települ és újraindul.
   Vagy **„Később"** → a következő bezáráskor magától települ.

> A **beállításaid és a licenckulcsod megmaradnak** a frissítés után — semmit nem kell újra megadni. (A program a felhasználói mappádban — `%APPDATA%\F1RaceEngineer\` — tárolja ezeket, amit a frissítés nem érint.)

A legfrissebb verzió manuálisan is letölthető (pl. új gépre):
**https://github.com/ZeroPointRace/F1-Race-engineer-releases/releases/latest**

---

### Egyéb problémák

Ha a fenti megoldások nem segítettek, írj a support-emailre és mellékeld a következőt:
- Mit csinált az alkalmazás pontosan (mit láttál, mit hallottál)
- Melyik F1 25 verziót használod (alap vagy 2026 DLC)
- Windows verzió (Win10 / Win11)

📧 **f1zeropointracing@gmail.com**

---

*F1 Race Engineer © 2026 ZeroPoint Racing — Minden jog fenntartva*
