---
layout: home
title: Zanke in spremenljivke
---

<script type="text/javascript" async
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

# Zanke

Če napišemo novo pop-uspešnico, v kateri brez predaha uporabljamo iste štiri akorde `C G a F`
in želimo to deliti s svojim kolegom, bo kar trajalo, da natipkamo celo pesem

`C G a F C G a F C G a F C G a F C G a F C G a F C G a F C G a F ... C G a F`

zato se znajdemo, prepoznamo vzorec, ki se ponavlja, in kolegu pošljemo

```
ponovi 50-krat:
    C G a F
```

Podobno je pri programiranju. Namesto da napišemo

```
pojdi v desno
pojdi v desno
pojdi v desno
pojdi v desno
pojdi v desno
```

poznajo tudi programski jeziki bližnjice, ki jim pravimo zanke. Na portalu Pišček so videti tako:

![pišček zanka](../slike/piscek_zanka.PNG)

Tu v zanki povemo, kolikokrat je treba ponoviti njeno vsebino. Kasneje bomo spoznali še drugi tip zank, ki jih uporabimo,
ko število ponovitev ni poznano v naprej, moramo pa ponavljati določene ukaze, dokler je izpolnjen neki pogoj,
npr.

```
dokler ne padeš čez rob sveta:
    pojdi v desno
```

Vendar bomo te zanke spoznali kasneje, saj bomo najprej spoznali pogojne stavke.

## Brez računalnika

### Barvanje mreže

Katere od [mrež](../gradiva_pdf/barvanje-mreze.pdf) (iz zaporedja ukazov) lahko pobarvamo tako, da ponavljamo kratko zaporedje ukazov?

## Naloge na Portalu Pišek

### [Slastna zrna](https://pisek.acm.si/contents/4907-905475276192595697-1358046987851793899-731188588614266740/)

Sprehodite se do zrna, a poskusite porabiti čim manj koščkov.

Ko rešiš nalogo za ⭐⭐, poskusi rešiti še nalogi za ⭐⭐⭐ in ⭐⭐⭐⭐.

### [Seprentina](https://pisek.acm.si/contents/4907-905475276192595697-1358046987851793899-678880300412440287/)

Pomagaj robotu priti do konca poti.

Ker je na voljo le malo delčkov, je zelo pomembno, da program sestavimo pametno. Razmisli, kakšen je vzorec, ki se ponovi.

Ko rešiš nalogo za ⭐⭐, poskusi rešiti še nalogi za ⭐⭐⭐ in ⭐⭐⭐⭐. Ne pozabi,
da lahko zanke **gnezdimo** - znotraj ene zanke lahko vstavimo drugo zanko.

### [Zmajček in cekini](https://pisek.acm.si/contents/4907-319805995281415931-895474193433606586-1672915584168735419-43613985217736079/)

Sprehodi zmajčka tako, da bo pobral vse cekine. Opaziš kakšne ponavljajoče se vzorce? Ali lahko cekine pobiraš tudi na drugačen način?

Ko rešiš nalogo za ⭐⭐, poskusi rešiti še nalogi za ⭐⭐⭐ in ⭐⭐⭐⭐. Ne pozabi,
da lahko zanke **gnezdimo** - znotraj ene zanke lahko vstavimo drugo zanko.

# Spremenljivke

Pogosto si moramo v programu kakšno vrednost zapomniti,
če jo želimo večkrat uporabiti. Za to uporabljamo spremenljivke. Vsaka spremenljivka ima svoje ime
(npr. $$x$$, `trenutna_vsota`, `ime`) in vrednost, ki jo hranimo v tej spremenljivki
(npr. $$3{.}14$$, $$21$$, `Bojan`). Ker so to _spremenljivke_, lahko njihove vrednosti spreminjamo.

Spremenljivke v večini programskih jezikov lahko poljubno poimenujemo, vendar je njihovo ime namenjeno zgolj programerju, saj ime spremenljivke navadno pove, kaj se v spremenljivki nahaja. Zato je dobra praksa, da spremenljivke poimenujemo smiselno. Na primer, če imamo neko spremenljivko, v katero si bomo shranjevali trenutno vsoto, je smiselno tudi spremenljivko poimenovati `trenutna_vsota`, čeprav je na nivoju računalnika čisto vseeno, če to spremenljivko poimenujemo `ime`.

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

Poskusite napisati diagram poteka in psevdo kodo, ki izračuna $$n$$-to Fibonaccijevo število.

### Evklidov algoritem

Pri tej nalogi boste s pomočjo Evklidovega algoritma poiskali največji skupni delitelj danih dveh števil.

Najprej se spomnimo kako Evklidov algoritem deluje. Začnemo z dvema številoma $$a$$ in $$b$$, za kateri želimo izračunati največji skupni delitelj. Število $$a$$ zapišemo kot $$a = q \cdot b + r$$, kjer je $$r$$ strogo manjši od števila $$b$$. Nato število $$a$$ nadomestimo z $$b$$ in $$b$$ nadomestimo z $$r$$. Postopek ponavljamo, dokler ne dobimo da je $$r=0$$. v tem primeru vemo, da je na tem koraku $$b$$ največji skupni delitelj prvotnih števil $$a$$ in $$b$$.

Na podoben način kot pri računanju Fibonaccijevega zaporedja tudi tukaj simulirajte algoritem s pomočjo dveh škatel, kjer za `manjše` uporabite število 57 in za `večje` uporabite število 81. Na koncu napišite diagram poteka in psevdo kodo.

### Palindrom

Palindrom je vsaka beseda, ki se enako prebere od spredaj in od zadaj.
Kako bi ugotovili, ali je beseda `kajak` palindrom? Kaj pa `fdfpokfgpdokvfdfvkodpgfkopfdf`?

Poskusite se spomniti algoritma, ki bo za vsako besedo znal povedati, ali je palindrom.

Napišite diagram poteka in psevdo kodo za ta algoritem.

## Naloge na Portalu Pišek

V tem sklupu bomo uporabo zank nadgradili s spremenljivkami.

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

**opomba:** Za barvanje kvadratka lahko uporabite kar blok izkoplji kovanček.
