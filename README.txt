# Konyhám – első működő verzió

## Mit tud?
- Készletkezelés hűtő, kamra és fagyasztó (külön fiókok) szerint
- Mennyiség, egység, kategória, lejárat, minimumkészlet, vonalkódmező
- Bevásárlólista: kizárólag a kipipált tételek kerülnek át a készletbe; az azonos termék mennyisége összeadódik
- Saját receptek, hozzávalók, elkészítés, adag, idő, fotó, kedvencek
- Recept-hozzávalók készlettel való összevetése
- Heti terv és hiányzó hozzávalók listázása
- Lejárati áttekintő, adatmentés és visszaállítás

## Ingyenes kipróbálás iPhone-on
A PWA telepítéséhez HTTPS-en elérhető webcím szükséges. A legegyszerűbb ingyenes út például egy GitHub Pages oldal:
1. Hozz létre egy GitHub-fiókot, majd egy új, nyilvános repository-t.
2. Töltsd fel a ZIP-ben lévő fájlokat a repository gyökerébe.
3. Settings → Pages → Deploy from a branch → main → /(root) → Save.
4. A létrejött HTTPS címet nyisd meg iPhone-on Safariban.
5. Megosztás → Főképernyőhöz adás.

A GitHub Pages használata ingyenes nyilvános statikus weboldalakhoz. A fiók létrehozása és feltöltése külön felhasználói művelet.

## Fontos iPhone-korlátok
- Az adatok a Safari/webalkalmazás helyi tárhelyén maradnak. Böngészőadat-törlés vagy eszközcsere adatvesztést okozhat, ezért használd rendszeresen a Beállítások → Biztonsági mentés funkciót.
- Az iOS webes értesítései verzió- és telepítési feltételekhez kötöttek. Ez a prototípus jelenleg megnyitáskor mutatja a lejáratokat; a garantált, háttérben futó lejárati értesítés nincs készre ígérve.
- A kamerás vonalkódolvasás csak akkor működik, ha a Safari támogatja a BarcodeDetector API-t és engedélyezed a kamerát. Kézi vonalkódmező mindig használható.
- A recept-hozzávalók összevetése egyszerű névegyezésen alapul, ezért az összetettebb mennyiségi egyezést később pontosítani kell.

## Adatvédelem
Nincs beépített felhős szinkronizálás vagy külső adatküldés. Az alkalmazás helyben, a böngésző localStorage tárhelyén tárolja az adatokat.
