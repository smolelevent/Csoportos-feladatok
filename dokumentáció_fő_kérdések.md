# <center>DOKUMENTÁCIÓ</center>
### <center>Készítők:</center>
<center>Kiss Levente, Szép Dániel, Szabó Richárd</center>

## 1. Mi a szoftver célja, a megoldandó probléma bemutatása
### <u>Mi a szoftver célja:</u>
A **Chatex** alkalmazás célja hogy egy alternatívát nyújtson a híres Messenger helyett, mégpedig úgy, hogy csak az egymás közötti csevegésre fókuszál minden olyan funkció nélkül, ami nem ezt a célt szolgálja. Más szóval, a **Chatex** használata egy sokkal könnyebb, gyorsabb, és felhasználó barátabb környezetet nyújt, míg ugyanúgy megtartja a játékos funkciókat. 

### <u>Megoldandó probléma bemutatása:</u>
**Chatex** alkalmazásunk a Messenger jelenlegi (v485.2.0.68.111) hibáit javítja ki, köztük a végpontok közötti titkosítástól való teljesítmény problémákat (a felhasználó dönthet a bekapcsolásáról) és a kezelő felületek inkonzisztens megjelenését egy egységes felülettel.

## 2. A szoftvernek milyen funkciókat kell megvalósítani
### <u>Tervezett funkciók:</u>
A **Chatex** 1.0-ra az alkalmazás tartalmazni fog: két lépcsős azonosítást, emojikat (a címzett azt az emojit kapja amit a feladó küldött), barátkérelmek, csoportok létrehozását. Ezek a funkciók lesznek a prioritásaink, amint az 1.0 elkészül.

## 3. A szoftverhez és az egyes funkciókhoz milyen szoftverkomponensek kellenek
A Chatex a Flutter framework használatával készül Dart programozási nyelvvel Android Studioban. Ebből kifolyólag elsősorban Androidra készül, de elérhető weben, és Windows-on is. A webes felület bővítve lesz PHP-val, CSS-el és JavaScript-el egyaránt. A regisztrált fiókok egy adatbázis szerverhez lesznek kötve, ahol külön jogosultságokkal fognak rendelkezni a felhasználók és az adminisztrátorok. Az adminisztrátoroknak egy külön felület lesz kialakítva az alkalmazáson belül, hogy közvetlenül tudják kezelni az adatokat (Windowsban is lesz erre lehetőség). A program külső könyvtárakat fog használni, illetve API-kat amelyekkel egy minőségi chat alkalmazás fog születni.

## 4. A szoftver működésének mik a műszaki feltételei
### <u>Android:</u>
Operációs rendszernek minimum az Android 5.0 (API 21) vagy újabbat el kell érnie.
Flutter támogatja az arm32, arm64, és x86_64 architektúrákat.