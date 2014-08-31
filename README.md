# A jegyszámítóról

A programot elsősorban azért hoztam létre, mert sokszor több percet kellett számolgatnom egy-egy dolgozat előtt, hogy legalább milyen jóra kell megírnom ahhoz, hogy egy bizonyos érték felett maradjon az átlagom.
Ezt a feladatot hivatott elvégezni a jegyszámító, amellyel könnyedén nyomon követheted az átlagaid alakulását, és előre tudod majd, hogy milyen eredményt kell elérned, hogy meglegyen az áhított átlag.

# A program használata

A jegyszámító tiszta JavaScriptre épül, így elméletileg a teljes oldal letöltése után lokálisan is használható, ez azonban egy-két funkciót elronthat, tipikusan ilyen a cookie-k kezelése, azaz az adatok elmentése.
Az oldal egyelőre folyamatos fejlesztés alatt áll, így komoly használatra még nem ajánlanám, az adatok megőrzése, vagy a különböző verziók közt a visszafele kompatibilitás nem garantált.

Tantárgy hozzáadása
-------------------
A táblázat legalsó sorában a `+ tantárgy` linkre kattintva egy felugró szövegmezőt látunk (ezt lehet, hogy külön kell engedélyezni a böngészőben), ebbe beírva a tantárgy nevét, majd az `OK` gombra kattintva az új sor megjelenik a táblázatban.

Jegy hozzáadása
---------------
A táblázatban minden tantárgy sorában a jegyek mellett találunk egy `+ jegy` linket, erre kattintva lehet az adott tantárgyhoz egy új jegyet hozzáadni.

Jegy módosítása
---------------
A táblázatban bármely jegyre kattintva a táblázat alatt megjelenik egy kis űrlap, melyben a jegy adatait módosíthatjuk, vagy ki is törölhetjük azt.

Bemeneti szöveg írása
---------------------
Ha valaki gyorsabb módszernek gondolja a bemeneti szöveg megírását a kattintgatásnál, erre is van lehetőség. A szintaktikája meglehetősen egyszerű, a tantárgy neve után egy kettőspont következik, ezt követően pedig szóközzel elválasztva a jegyek. A jegyek a következő formátumban kerülnek megadásra: először a jegy típusának kezdőbetűje, majd a jegy értéke. Az egyes tantárgyi szekciók egy `|` jellel vannak elválasztva. Minderre egy példa:

    földrajz: v3 n3 k2 | matematika: t3 d4 t3/4 | történelem: k1 n4 t3

(Megjegyzés: az utolsó tantárgy után opcionálisan írható egy lezáró `|` is).


# Ismert hibák és tökéletlenségek

* A cookies adatmentés nem működik
* A jegyek megadása egyelőre nem túl felhasználóbarát
* Promptokban a "mégse" nyomása furcsa hibákat tud okozni
