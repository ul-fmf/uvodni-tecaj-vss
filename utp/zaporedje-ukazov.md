---
layout: home
title: Zaporedje ukazov
---

Kot boste spoznali, računalniki vedno naredijo točno to, kar jim naročimo - kar pa ni vedno tisto, kar smo imeli v mislih.
Če bi npr. računalnik vprašali _Ali lahko vprašam, koliko je ura?_, bi dobili odgovor _Da._

Večina programov za svoje izvajanje prejme informacije ali vrednosti, ki jim rečemo vhodni podatki.
Najpogosteje program te podatke sprejme od zunaj, na primer od uporabnika.
Primer: predstavljajte si, da pišete program za kalkulator. Vhodni podatki za ta program bi bili števila in operacije, ki jih želi uporabnik izvesti.
Če želi uporabnik sešteti števili 5 in 3, bi bili vhodni podatki za program število 5, število 3 in operacija "seštevanje".

Primer programa, ki ne sprejme nobenih vhodnih podatkov bi bil lahko kalkulator, ki vedno zmnoži števili 6 in 7, ali pa program,
ki na sredino zaslona vedno nariše krog s polmerom 100 točk.
Na začetku tega tečaja se boste najprej spoznali z res enostavnimi programi, ki ne sprejmejo vhodnih podatkov.

Ko zapišemo svoj program, t.j. neko zaporedje ukazov, je koristno preveriti, kako se bo program izvajal po korakih.
Če se program ustavi za vsake vhodne podatke, in to s pravilnim rezultatom, rečemo, da program reši problem,
oz. da je program pravilen. Nepravilen program se ne ustavi na vseh vhodnih podatkih ali pa za nekatere da napačen rezultat.

## Brez računalnika

Pri teh nalogah imate priložnost, da se postavite v vlogo računalnika - izvajalca ukazov.
To je pomemben del veščine programiranja, saj vam pomaga razumeti, kako bo vaš program dejansko deloval.

### Risanje po navodilih

Pri tej nalogi uporabniki dajejo izvajalcem navodila za risanje enostavne slike.
Pomembno je, da izvajalci slike ne vidijo vnaprej.
Izvajalci naj sledijo navodilom, ampak naj poskusijo uporabnike pripraviti do tega, da podajo bolj natančna navodila.

### Kako pridemo do računalniške učilnice

Zdaj, ko imate že nekaj izkušenj z dajanjem natančnih navodil: kako bi podali čim bolj podroben opis poti od vhoda v stavbo do računalniške učilnice?

### Barvanje mreže

Napišite programe, s katerimi boste pobarvali mreže v [priloženi datoteki](barvanje-mreze.pdf).
Začnite v zgornjem levem polju. Na voljo imate ukaze:

- premakni se za ena na desno,
- premakni se za ena na levo,
- premakni se za ena navzdol,
- premakni se za ena navzgor in
- pobarvaj kvadratek.

Kaj pomeni, če spremenimo vrstni red ukazov - ali vedno dobimo napačen rezultat?
Kako se spremeni program, če spremenimo začetno polje?
Kaj naj se zgodi, če zaidemo iz mreže?

### Otok zakladov

To nalogo smo si izposodili s portala [Vidra](http://vidra.si/otok-zakladov/). Za igro potrebujemo gusarja ter sedem udeležencev, ki predstavljajo otočane in gusarja usmerjajo.
Gusarjeva naloga je poiskati otok zakladov.

Otočani dobijo listek z imenom svojega otoka ([gusarji-otoki.pdf](gusarji-otoki.pdf)), in navodila kam iz njihovega otoka odpotuje ladja A in kam ladja B.
Gusar dobi prazen zemljevid ([gusarji-prazen-zemljevid.pdf](gusarji-prazen-zemljevid.pdf)), na katerem so narisani vsi otoki, ni pa napisano kam lahko iz posameznega otoka odpluje.
Gusar svojo pot začne na Otoku gusarjev.

## Naloge na Portalu Pišek

### [Pišek zoba zrna](https://pisek.acm.si/contents/4907-4902-6586947264732270-337559782458156072-792990685659790508-1406670246764682841/)

Sestavite zaporedje ukazov, s katerim bo Pišek pozobal vsa zrna.
Možnih je več rešitev problema - ali lahko najdete različne?
Koliko je najmanjše možno število ukazov, s katerimi še lahko rešimo nalogo?

Za utrjevanje rešite vajo [Spoznaj Piška in jajca](https://pisek.acm.si/contents/4907-4902-6586947264732270-1019917885797944638-500716107770886984/).

### [Zajček se pase](https://pisek.acm.si/contents/4907-319805995281415931-598127356695689187-1377786176696507594-39813363471970577-194969246516065149/)

Dane ukaze razvrstite v ustrezen vrstni red, da bo zajček pozobal vse deteljice.

### [Gusarji iščejo zaklad](https://pisek.acm.si/contents/4907-319805995281415931-1468740812716735939-1065261577502713763-1001406523172202844/)

Najprej si dobro oglejte sliko in poiščite otok z zakladom.  
Ladjo lahko do otoka pripeljemo na več različnih načinov.
Pri tej nalogi ni nobene omejitve glede števila delčkov, ki jih lahko uporabite, zato imate pri pisanju programa proste roke.
Kljub temu poskusite poiskati čim krajšo pot. Ko se odločite za pot, delčke nanizajte v pravo zaporedje.

### [Neža barva](https://pisek.acm.si/contents/4907-319805995281415931-1468740812716735939-1065261577502713763-494973846763652249/)

Dobro si oglejte sliko in razmislite, kaj zahteva naloga. Opazimo lahko, da moramo voščenko najprej premakniti za eno polje v levo,
nato pa lahko začnemo s premikanjem po stranicah 6-kotnika, pri čemer vsako stranico pobarvamo rdeče.
Premikamo se lahko v smeri urinega kazalca, ali pa ravno obratno.

Na delovni površini so razmetani vsi delčki, ki jih potrebujete.
Čeprav bi se po mreži lahko premikali v kateri koli smeri, delčki na delovni površini nakazujejo rešitev v nasprotni smeri urnega kazalca.

### [Sprehod po džungli](https://pisek.acm.si/contents/4907-905475276192595697-1211536570574997293-916355264606378407/)

Pomagajte taborniku Tinetu, ki želi obiskati vsak košček džungle.
Pozor - pri tej nalogi so ukazi drugačni! Namesto premikov glede na smeri v mreži, se Tine premika v smer, kamor je trenutno obrnjen.
Če gleda v desno in se želi premakniti gor, se mora torej najprej obrniti v levo, nato pa se premakniti naprej.

Kot vidite, je program odvisen od nabora ukazov, ki ga imamo na voljo.
Poskusite sestaviti program, ki uporabi ukaze iz prejšnjih nalog (gor, dol, levo in desno) in ga primerjajte z rešitvijo te naloge.

### Delovni list

Rešite [delovni list](delovni-list-01.pdf).

### Naloge za samostojno reševanje

- [Pozabljena zrna](https://pisek.acm.si/contents/4907-905475276192595697-1211536570574997293-749187630887873442/)
- [Začetni koraki](https://pisek.acm.si/contents/4907-905475276192595697-1211536570574997293-156249197232542929/): podobno kot zgoraj, a omejitev števila delčkov pride do izraza
- [Gozdno sankališče](https://pisek.acm.si/contents/4907-905475276192595697-1211536570574997293-761725721677256299/)
