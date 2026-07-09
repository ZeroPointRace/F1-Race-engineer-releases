# Változásnapló — F1 ZeroPoint Race Engineer

Az egyes kiadások **felhasználói szintű** újdonságai és javításai. A legújabb verzió felül.

> Munka közben az új sorokat a **`## [Kiadatlan]`** szekcióba írjuk. Kiadáskor ez
> átnevezésre kerül a verziószámra, és automatikusan felkerül a Manual repóba.

## [Kiadatlan]
- (a következő kiadás újdonságai ide kerülnek)

## v1.0.10 — 2026-07-09
- 🚦 **Govee zászlófény támogatás:** a Govee okoslámpád valós időben jelzi a verseny-zászlókat (zöld, sárga a saját szektorodban, kék, piros, Safety Car). A Beállítások menüben kiválaszthatod a lámpát, és eseményenként állíthatod a színt, fényerőt és a villogást.
- 🌬️ **Szélszimulátor támogatás:** sebességgel arányos szél Arduino + ventilátorokkal, a Beállítások menüben konfigurálható (port, sebesség-tartomány, erősség).

## v1.0.9 — 2026-06-26
- 🔒 **Megbízhatóbb, offline is működő licencvédelem:** a licenc és a próbaverzió ellenőrzése mostantól kriptográfiailag aláírt kulcson alapul — internet nélkül is stabilan működik (max. 30 napig offline), és csak valódi visszavonáskor áll le. Frissítés után egyszer szükséges internetkapcsolat.
- 🌐 Az „internet szükséges" üzenet immár minden támogatott nyelven megjelenik.

## v1.0.8 — 2026-06-21
- 🔑 **Megbízhatóbb licenc/próbaverzió:** egy átmeneti internetkimaradás már nem zár ki — a program offline is működik (a próbaverzió a hátralévő napokig, az aktivált licenc 30 napig), és csak valódi licenc-visszavonáskor áll le.

## v1.0.7 — 2026-06-20
- 🌐 **PC IP a főmenüben induláskor:** a géped IP-címe már rögtön indításkor megjelenik (eddig csak a Verseny nézet megnyitása után jött elő).
- 🪟 **Windows 11 kompatibilitás:** a licenc-aktiválás és a próbaverzió az újabb Windows 11-eken (24H2) is megbízhatóan működik.

## v1.0.6 — 2026-06-19
- 🛠️ **Hibabejelentő gomb:** ha valami nem működik, a főmenüből egy kattintással elküldheted a naplót a támogatásnak — így gyorsabban tudunk segíteni.

## v1.0.5 — 2026-06-13
- 💬 Discord közösségi gomb a főmenüben.
- 🇬🇧 Az angol nyelvű hangos versenymérnök mostantól teljes — minden tanács angolul is megszólal.
- 🔧 Kisebb javítások (nyelv-oldal megjelenés).

## v1.0.4 — 2026-06-11
- 🔧 Kisebb hibajavítások.

## v1.0.3 — 2026-06-07
- 🔔 **Frissítés-sáv:** az app már AKKOR szól, amint új verzió elérhető (nem csak letöltés után), mutatja a letöltés állapotát, és kínálja az „Újraindítás most / Később" választást.
- 📜 **Verziókövetés:** minden kiadás újdonságai megjelennek a frissítés-sávban és a Manual oldalon.

## v1.0.2 — 2026-06-07
- 🔄 **Automatikus frissítés:** az alkalmazás magától észleli, letölti és telepíti az új verziókat — nincs többé kézi letöltés.
- 🔢 A verziószám a bal alsó sarokban mindig az **aktuális telepített verziót** mutatja.

## v1.0.1 — 2026-06-07
- 📋 A főmenüben a **„PC IP másolása"** gomb mostantól működik (egy kattintással beilleszthető az F1 25 telemetria-beállításába).

## v1.0.0 — 2026-06-07
- 🎉 **Első nyilvános kiadás.**
- 🔊 **Magyar hangos versenymérnök** (és további nyelvek), valós idejű tanácsokkal.
- 🗺️ Élő pályatérkép, telemetria-dashboard, stratégia- és gumikezelési javaslatok.
- 🏎️ F1 25 + 2026-os DLC (24 autó, Overtake/Boost) támogatás.
- 🎮 Kormány-gombokra köthető hangos lekérdezések (időjárás, stratégia, szomszéd autók).
