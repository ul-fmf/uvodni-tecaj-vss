---
layout: home
title: Spremenljivke
---

<script type="text/javascript" async
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

Pogosto si moramo v programu kakšno vrednost zapomniti,
če jo želimo večkrat uporabiti. Za to uporabljamo spremenljivke. Vsaka spremenljivka ima svoje ime
(npr. $$x$$, `trenutna_vsota`, `ime`) in vrednost, ki jo hranimo v tej spremenljivki
(npr. $$3{.}14$$, $$21$$, `Bojan`). Ker so to _spremenljivke_, lahko njihove vrednosti spreminjamo.

Spremenljivke v večini programskih jezikov lahko poljubno poimenujemo, vendar je njihovo ime namenjeno zgolj programerju, saj ime spremenljivke navadno pove, kaj se v spremenljivki nahaja. Zato je dobra praksa, da spremenljivke poimenujemo smiselno. Naprimer, če imamo neko spremenljivko, v katero si bomo shranjevali trenutno vsoto, je smiselno tudi spremenljivko poimenovati `trenutna_vsota`, čeprav je na nivoju računalnika čisto vseeno, če to spremenljivko poimenujemo `ime`.

## Brez računalnika

### Fibonaccijevo zaporedje

Verjetno ste že kdaj slišali za Fibonaccijevo zaporedje. To je zaporedje, kjer sta prvi in drugi člen enaka 1, vsak naslednji člen pa je vsota prejšnjih dveh. Pri tej vaji boste simulirali računalnik, ki računa števila Fibonaccijevega zaporedja.

V krogu si podajajte dve škatli. Na eni piše `manjše` in na drugi `večje`. V teh dveh škatlah se nahajata dve števili. Vaša naloga je sledeča:

1. Pogledate števili v obeh škatlah,
2. seštejete števili in rezultat napišete na nov listek,
3. listek z najmanjšim številom odstranite,
4. preostala dva listka razvrstite v ustrezno škatlo,
5. predjate škatli svojemu sosedu.

Na ta način poiščite prvo Fibonaccijevo število, ki je večje od 1000.

Poskusite napisati psevdo kodo, ki izračuna $$n$$-to Fibonaccijevo število.

### Evklidov algoritem

Pri tej nalogi boste s pomočjo Evklidovega algoritma poiskali največji skupni delitelj danih dveh števil.

Najprej se spomnimo kako Evklidov algoritem deluje. Začnemo z dvema številoma $$a$$ in $$b$$, za kateri želimo izračunati največji skupni delitelj. Število $$a$$ zapišemo kot $$a = q \cdot b + r$$, kjer je $$r$$ strogo manjši od števila $$b$$. Nato število $$a$$ nadomestimo z $$b$$ in $$b$$ nadomestimo z $$r$$. Postopek ponavljamo, dokler ne dobimo da je $$r=0$$. v tem primeru vemo, da je na tem koraku $$b$$ največji skupni delitelj prvotnih števil $$a$$ in $$b$$.

Na podoben način kot pri računanju Fibonaccijevega zaporedja tudi tukaj simulirajte algoritem s pomočjo dveh škatel, kjer za `manjše` uporabite število 57 in za `večje` uporabite število 81.

### Palindrom

Palindrom je vsaka beseda, ki se enako prebere od spredaj in od zadaj.
Kako bi ugotovili, ali je beseda `kajak` palindrom? Kaj pa `fdfpokfgpdokvfdfvkodpgfkopfdf`?

Poskusite se spomniti algoritma, ki bo za vsako besedo znal povedati, ali je palindrom.

Napišite prevdo kodo za ta algoritem.

## Naloge na Portalu Pišek

V tem sklupu bomo uporabo zank nadgradili s spremenljivkami. Prav tako se boste pri tem sklopu spoznali z _vhodom_
(s katerega lahko program bere) in _izhodom_
(kamor lahko program piše). Vhod in izhod sta zelo pomembna, saj preko njiju računalnik komunicira z zunanjim svetom.

Preprost primer programa, ki uporablja vhod in izhod,
je _Računalo_. Vanj vnašamo (preko vhoda) števila in
operacije, računalo pa nam na svojem izhodu zapiše
rezultat, ki ga iščemo.

Če programi ne bi mogli brati z vhoda in pisati na izhod,
bi bila njihova uporaba zelo omejena.

### [Geslo za raketo](https://pisek.acm.si/contents/4907-905475276192595697-336263441319752813-263757501836633867/)

Pri tej nalogi moramo število, ki ga najdemo na polju, prebrati in shraniti v robotov spomin, nato pa ga zapisati na neko drugo predpisano polje.

Na drugem in tretjem nivoju moramo prebrati 2 oz. 3 števila
ter na predpisano polje zapisati njuno/njihovo vsoto.

### [Koordinate](https://pisek.acm.si/contents/4907-905475276192595697-336263441319752813-1402538532350177809/)

_Za reševanje te naloge je treba poznati zanke._

To je težja različica naloge _Geslo za raketo_, saj moramo vse, kar smo pri _Geslu za raketo_ naredili le enkrat, tukaj opraviti večkrat, pri čemer si pomagamo z zankami.

Na prvi stopnji moramo tako 5-krat prepisati število,
na drugi in tretji stopnji pa moramo 5-krat na ciljno polje zapisati vsoto nekaj števil.

Na tretji stopnji se vam zanko splača uporabiti tudi že pri samem branju, saj je treba izračunati vsoto petih števil.

### [Zmajček barva in šteje](https://pisek.acm.si/contents/4907-905475276192595697-336263441319752813-192594086067387490/)

_Za reševanje te naloge je treba poznati zanke._

Zmajček mora najprej prebrati število, ki ga sreča na enem od polj, nato pa izkopati toliko kovancev, kot je bila vrednost števila. Zato si mora vrednost števila
zapomniti in jo shraniti v spremenljivko.

Na drugem nivoju so kovančki razporejeni v pravokotnik,
na tretjem pa v trikotnik, kar nalogo nekoliko oteži.

### [Računanje](https://pisek.acm.si/contents/4907-905475276192595697-336263441319752813-608309524412854214/)

Na prvih dveh nivojih nas čakata delno napisana programa, ki prebereta dve števili z vhoda.
Programa morata na izhod izpisati ustrezen rezultat (vsoto in produkt) teh dveh števil. Na tretjem nivoju je naloga podobna, le da moramo program napisati čisto od začetka.

### [Aritmetična zaporedja](https://pisek.acm.si/contents/4907-905475276192595697-336263441319752813-1321351274884031317/)

_Za reševanje naloge na tretji stopnji je treba poznati zanke._

Zaporedje $$a_1, a_2, a_3, ...$$ je aritmetično, če je
razlika med zaporednima členoma zaporedja vedno enaka.
Primeri aritmetičnih zaporedij so

- 1, 3, 5, 7 ... (razlika je vedno 2),
- 2, 5, 8, 11 ... (razlika je vedno 3),
- 5, 2, -1, -4 ... (razlika je vedno -3).

Aritmetično zaporedje je tako povsem določeno s svojim
začetnim členom $$a_1$$ in razliko med zaporednima členoma, ki jo označimo z $$r$$.

Na prvi stopnji moramo popraviti program, ki prebere z vhoda $$a_1$$ in razliko $$r$$, na izhod pa mora zapisati $$a_{10}$$, tj. deseti člen zaporedja: $$a_{10} = a_1 + 9r$$.

Na drugi stopnji mora program prebrati z vhoda še število $$i$$ in na izhod zapisati $$i$$-i člen zaporedja, ki ga dobimo po formuli $$a_i = a_1 + (i - 1) r$$.

Na tretji stopnji je vhod enak kot pri drugi, program pa mora na izhodu zapisati prvih $$i$$ členov, tj. $$a_1, a_2, \dots, a_i$$.

### [Trikotniki](https://pisek.acm.si/contents/4907-905475276192595697-336263441319752813-1107968706648330591/)

Na prvi stopnji je treba izračunati tretji kot v trikotniku: `TRETJI = 180 - (PRVI + DRUGI)`.

Za drugo in tretjo stopnjo potrebujemo pogojne stavke, zato se nanju vrnite po naslednjem sklopu.

### Naloge za zagrete

_Za reševanje teh nalog je treba poznati pogojne stavke, zanke, včasih tudi tabele in še kaj._

- [Pišček raziskuje](https://pisek.acm.si/contents/4907-905475276192595697-336263441319752813-1228907312687806211/): sledi sledem, ki jih najdeš na poljih in poberi vsa zrna
- [Taborniška skupina Ogenj](https://pisek.acm.si/contents/4907-905475276192595697-336263441319752813-299337302389322177/): Preštej število tabornikov, katerih starost je enaka zahtevani.
- [Taborniška skupina Medved](https://pisek.acm.si/contents/4907-905475276192595697-336263441319752813-1635014616559399342/): Preštej število tabornikov, ki so starejši od predpisane meje.
