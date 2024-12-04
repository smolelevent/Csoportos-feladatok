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
A telefon operációs rendszerének minimum az Android 5.0-át (API 21) vagy újabbat kell futtatnia. Emellett mind az arm32-es, arm64-es, és a x86_64-es architektúrákat kell hogy támogassa.

### <u>Windows:</u>
A gép operációs rendszerének minimum Windows 10-et (64 bit) kell futtatnia, és szükség van a Flutter projekt futtatásakor települő Windows SDK (már a Flutterel feltelepűl).

### <u>Web:</u>
A Flutter alkalmazások futtatása weben szűk böngésző támogatással rendelkeznek ezek a következők: Google Chrome (Chromium, fejlesztői eszközök), Microsoft Edge (Chromium), és a Mozilla Firefox (iOS-re való fejlesztéskor Safari is engedélyezett). A böngészőknek támogatnia kell a WebAssembly compliert, mely az alkalmazás futását hajtja végre (renderelés: CanvasKit-el, HTML-el történhet).

### <u>Fejlesztői eszközök:</u>
- Androidra való fejlesztéshez szükség van egy IDE-re, mi esetünkben az Android Studio-ra, azon belül az Android SDK-ra mellyel nem kapnánk végprogramot és hogy ezt láthatsuk egy Emulatorra (lehet fizikai eszköz is, illetve virtuális készülék).

- Windowshoz ajánlott a Visual Studio használata, illetve a "Desktop development with C++" csomagot letölteni, de a csomag letöltése után mi az Android Studionál maradunk.

- Webhez való fejlesztéshez a Flutter DevTools használata ajánlott, ami Chrome-al társítva még több fejlesztői eszközt eredményez.

*Mind a 3 féle fejlesztés kezelhető a Flutter terminálján keresztűl.*

### <u>Összegzés táblázatban:</u>
| **Platform** |    **Minimum OS**   |    **Fejlesztési eszközök**   | **Támogatott Architektúrák** |
|:------------:|:-------------------:|:-----------------------------:|:----------------------------:|
|    Android   |     Android 5.0+    |  Android Studio, Android SDK  |     arm32, arm64, x86_64     |
|    Windows   | Windows 10, 64-bit+ |   Visual Studio, Windows SDK  |            x86_64            |
|      Web     |   Modern böngészők  | Chrome, Firefox, Edge, Safari |       WebAssembly-alapú      |