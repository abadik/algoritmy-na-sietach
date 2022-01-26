Algoritmy na sieťach 2022 - Python
=====

# Obsah
- [Algoritmy na sieťach 2022 - Python](#algoritmy-na-sieťach-2022---python)
- [Obsah](#obsah)
- [Inštalácia - Python](#inštalácia---python)
- [Inštalácia - IDE](#inštalácia---ide)
- [Užitočné VS Code rozšírenia](#užitočné-vs-code-rozšírenia)
- [Úvod do jazyka Python](#úvod-do-jazyka-python)
  - [Operátory](#operátory)
    - [Sčítanie](#sčítanie)
    - [Odčítanie](#odčítanie)
    - [Násobenie](#násobenie)
    - [Delenie](#delenie)
    - [Celočíselné delenie](#celočíselné-delenie)
    - [Umocňovanie](#umocňovanie)
    - [Modulo](#modulo)
    - [Je rovný](#je-rovný)
    - [Nie je rovný](#nie-je-rovný)
    - [Menší než (väčší než)](#menší-než-väčší-než)
    - [Menší alebo rovný (väčší alebo rovný)](#menší-alebo-rovný-väčší-alebo-rovný)
    - [A zároveň](#a-zároveň)
    - [Alebo](#alebo)
    - [Negácia](#negácia)
  - [Základné typy údajov](#základné-typy-údajov)
    - [Boolovská hodnota `bool`](#boolovská-hodnota-bool)
    - [Celé čísla `int`](#celé-čísla-int)
    - [Desatinné čísla `float`](#desatinné-čísla-float)
    - [Znakové reťazce (string) `str`](#znakové-reťazce-string-str)
  - [Premenné a priradenie](#premenné-a-priradenie)
    - [Priraďovací príkaz](#priraďovací-príkaz)
    - [Pretypovanie hodnôt](#pretypovanie-hodnôt)
  - [For-cyklus](#for-cyklus)
    - [Príklady](#príklady)
    - [Funkcia `range()`](#funkcia-range)
    - [Vnorené cykly](#vnorené-cykly)
  - [Podmienky](#podmienky)
    - [Príklady](#príklady-1)
  - [Podmienený cyklus](#podmienený-cyklus)
    - [Príklady](#príklady-2)
  - [Funkcie](#funkcie)
    - [Príklady](#príklady-3)
  - [Moduly](#moduly)
    - [Modul `math`](#modul-math)
  - [Operácia indexovania `[]`](#operácia-indexovania-)
  - [Zoznam `list`](#zoznam-list)
    - [Indexovanie](#indexovanie)
    - [Zreťazenie](#zreťazenie)
    - [Viacnásobné zreťazenie](#viacnásobné-zreťazenie)
    - [Zisťovanie prvku](#zisťovanie-prvku)
    - [Prechádzanie prvkov zoznamu](#prechádzanie-prvkov-zoznamu)
    - [Zmena hodnoty prvku zoznamu](#zmena-hodnoty-prvku-zoznamu)
    - [Štandardné funkcie so zoznamami](#štandardné-funkcie-so-zoznamami)
    - [Funkcia `list()`](#funkcia-list)
    - [Rezy `slice`](#rezy-slice)
    - [Metóda `count()`](#metóda-count)
    - [Metóda `index()`](#metóda-index)
    - [Metóda `append()`](#metóda-append)
    - [Metóda `pop()`](#metóda-pop)
    - [Metóda `insert()`](#metóda-insert)
    - [Metóda `remove()`](#metóda-remove)
    - [Metóda `sort()`](#metóda-sort)
  - [n-tica `tuple`](#n-tica-tuple)
    - [Funkcia `enumerate()`](#funkcia-enumerate)
  - [Slovník `dict`](#slovník-dict)
- [Python dokumentácia](#python-dokumentácia)
- [Modul `pandas` dokumentácia](#modul-pandas-dokumentácia)
- [Modul `NetworkX` dokumentácia](#modul-networkx-dokumentácia)
- [Modul `mathplotlib` dokumentácia](#modul-mathplotlib-dokumentácia)

# Inštalácia - Python
Stiahnite si najnovšiu verziu Python: https://python.org/

Návod na inštaláciu nájdete tu: https://youtu.be/hjYF_WRrreQ?t=306

**Nezabudnite zaškrtnúť `Add Python 3.X to PATH`!**

# Inštalácia - IDE
Jedná sa o akýsi textový editor s užitočnými funkciami.

Budeme používať *Visual Studio Code*. (Návod na stiahnutie a inštaláciu: https://youtu.be/deLvhbagt5U?t=173)

Alternatívy:
- SublimeText (https://www.sublimetext.com/download)
- PyCharm (https://www.jetbrains.com/pycharm/download)

# Užitočné VS Code rozšírenia
- Python
- MagicPython
- Jupyter
- Jupyter Notebook Renderers
- vscode-icons
- Rainbow Brackets

# Úvod do jazyka Python
## Operátory
### Sčítanie
```Python
1 + 2
```
### Odčítanie
```Python
5 - 3
```
### Násobenie
```Python
2 * 3
```
### Delenie
```Python
5 / 2
```
Vráti desatinné číslo.
### Celočíselné delenie
```Python
1 // 2
```
Vráti celú časť po delení.
### Umocňovanie
```Python
3 ** 2
```
Umocňovanie - v tomto prípade $3^2$.
### Modulo
```Python
10 % 3
```
Vráti zvyšok po delení.
### Je rovný
```Python
1 == 1
```
### Nie je rovný
```Python
1 != 1
```
### Menší než (väčší než)
```Python
1 < 2
1 > 2
```
### Menší alebo rovný (väčší alebo rovný)
```Python
1 <= 2
1 >= 2
```
### A zároveň
```Python
1 < 2 and 2 < 3
```
### Alebo
```Python
1 < 2 or 2 > 3
```
### Negácia
```Python
not 1 < 2
```

## Základné typy údajov
### Boolovská hodnota `bool`
```Python
>>> type(True)
<class 'bool'>
```

### Celé čísla `int`
```Python
>>> type(123)
<class 'int'>
```
### Desatinné čísla `float`
```Python
>>> type(22 / 7)
<class 'float'>
```
### Znakové reťazce (string) `str`
```Python
>>> type('test')
<class 'str'>
```
```Python
>>> type("test")
<class 'str'>
```

## Premenné a priradenie
Premenná vzniká nie zadeklarovaním a spustením programu (ako v Pascale a v C), ale vykonaním priraďovacieho príkazu (nejakej existujúcej hodnote sa priradí meno).

**Meno premennej:**

-  môže obsahovať písmená, číslice a znak podčiarkovník,
-  pozor na to, že v Pythone sa rozlišujú malé a veľké písmená (case sensitive),
-  musí sa líšiť od pythonovských príkazov, tzv. *rezervovaných* slov (napr. `for`, `if`, `def`, `return`, `type`, …).

### Priraďovací príkaz
```Python
>>> a = 17
>>> b = "abcd"
>>> x = a
>>> b = 3.2
>>> a = a + 3
>>> a += 3      # a = a + 3
>>> print(a)
20
```

Paralelné priradenie
```Python
>>> a, b = 17, "abcd"
```


### Pretypovanie hodnôt
Mená typov `int`, `float` a `str` zároveň súžia ako mená pretypovacích funkcií, ktoré dokážu z jedného typu vyrobiť hodnotu iného typu.
```Python
>>> int(3.4)
3
>>> int("37")
37
>>> float(33)
33.0
>>> float("3.4")
3.4
>>> str(33)
"33"
>>> str(3.4)
"3.4"
```

## For-cyklus
### Príklady
```Python
for i in range(5):
    # opakované príkazy 
    print(i)
```

```Python
for i in range(2,5):
    # opakované príkazy 
    print(i)
```

```Python
for i in "Algoritmy", "na", "sieťach":
    # opakované príkazy 
    print(i)
```

```Python
for i in "Python":
    # opakované príkazy 
    print(i)
```

### Funkcia `range()`

`range(stop)`

`range(start, stop)`

`range(start, stop, step)`

*Parametre:*

- `start` prvý prvok vygenerovanej postupnosti (default `0`),
- `stop` hodnota, na ktorej sa už generovanie ďalšej hodnoty postupnosti zastaví - táto hodnota už v postupnosti nebude,
- `step` hodnota, o ktorú sa zvýši každý nasledovný prvok postupnosti (default `1`).

### Vnorené cykly
```Python
for i in "Python":
    # opakované príkazy
    for j in range(5):
        # iné opakované príkazy 
        print(f"Písmeno: {i}, číslo: {j}")
    # aj sem môžu ísť opakované príkazy
```

## Podmienky
### Príklady
```Python
body = 56
if body >= 60:
    print("Dostatočný počet bodov")
else:
    print("Nedostatočný počt bodov")
```
---

```Python
body = 56
if body >= 60:
    print("Máš dostatočný počet bodov")
```
`else` vetva nemusí existovať. Ekvivalentne môžeme zapísať nasledovne:
```Python
body = 56
if body >= 60:
    print("Máš dostatočný počet bodov")
else:
    pass
```
---

```Python
body = 56
if body >= 90:
    print(f"za {body} bodov získavaš známku A")
else:
    if body >= 80:
        print(f"za {body} bodov získavaš známku B")
    else:
        if body >= 70:
            print(f"za {body} bodov získavaš známku C")
        else:
            if body >= 60:
                print(f"za {body} bodov získavaš známku D")
            else:
                if body >= 50:
                    print(f"za {body} bodov získavaš známku E")
                else:
                    print(f"za {body} bodov získavaš známku Fx")
```
Ekvivalentne môžeme zapísať nasledovne:
```Python
body = 56
if body >= 90:
    print(f"za {body} bodov získavaš známku A")
elif body >= 80:
    print(f"za {body} bodov získavaš známku B")
elif body >= 70:
    print(f"za {body} bodov získavaš známku C")
elif body >= 60:
    print(f"za {body} bodov získavaš známku D")
elif body >= 50:
    print(f"za {body} bodov získavaš známku E")
else:
    print(f"za {body} bodov získavaš známku Fx")
```

## Podmienený cyklus
### Príklady
```Python
i = 0
while i < 20:
    print(i)
    i += 1 
```
---
```Python
i = 0
while i < 20:
    print(i)
    i += 1 
    if i == 10:
        break
```

## Funkcie
### Príklady
```Python
def meno_funkcie():
    # sem môžu ísť príkazy
```
---
```Python
def meno_funkcie():
    # sem môžu ísť príkazy
    return "výsledok"
```
---
```Python
def sucet(a, b):
    return a + b
```
---
```Python
def sucet(a, b = 1):
    return a + b
```

## Moduly
Ak potrebujeme pracovať s nejakým modulom, musíme to najprv Pythonu oznámiť špeciálnym spôsobom. Slúži na to príkaz `import`.

### Modul `math`
Pomocou takéhoto zápisu:
```Python
import math
```
umožníme našim programom pracovať s matematickými funkciami z tejto knižnice. V skutočnosti týmto príkazom Python vytvorí novú premennú `math` (nové meno v pamäti mien premenných).

Knižnica v tomto module obsahuje, napríklad tieto matematické funkcie: `sin()`, `cos()`, `sqrt()`. Lenže s takýmito funkciami nemôžeme pracovať priamo: Python nepozná ich mená, pozná jediné meno a to meno modulu `math`. Keďže tieto funkcie sa nachádzajú práve v tomto module, budeme k nim pristupovať, tzv. bodkovou notáciou (dot notation): za meno modulu uvedieme prvok (v tomto prípade funkciu) z daného modulu. Napríklad `math.sin()` označuje volanie funkcie sínus a `math.sqrt()` označuje výpočet druhej odmocniny čísla.

```Python
import math
a = math.sin(1)
print(a)
```

## Operácia indexovania `[]`
Pomocou tejto operácie vieme pristupovať k jednotlivým znakom postupnosti (znakový reťazec je postupnosť znakov). Jej tvar je `reťazec[číslo]`.

Celému číslu v hranatých zátvorkách hovoríme index:

- znaky v reťazci sú indexované od `0` do `len()-1`, t.j. prvý znak v reťazci má index `0`, druhý `1`, … posledný má index `len()-1`,
- výsledkom indexovania je vždy 1-znakový reťazec (čo je nový reťazec s kópiou 1 znaku z pôvodného reťazca) alebo chybová správa, keď indexujeme mimo znaky reťazca.

```Python
abc = 'Toto je Python'
print(abc[4])           # vypíše " " (medzeru)
print(abc[len(abc)-1])  # vypíše "n"
print(abc[-3])          # vypíše "h"
print(abc[:-10])        # vypíše "Toto"
print(abc[-6:])         # vypíše "Python"
print(abc[5:-7])        # vypíše "je"
print(abc[2:10:2])      # čo vypíše? (posledné čslo je krok)
```

## Zoznam `list`
Dátová štruktúra zoznamu sa v Pythone volá `list`.

```Python
teploty = [10, 13, 15, 18, 17, 12, 12]
nakup = ['chlieb', 'mlieko', 'rozky', 'jablka']
studenti = ['Juraj Janosik', 'Emma Drobna', 'Ludovit Stur', 'Pavol Habera', 'Margita Figuli']
zviera = ['pes', 'Dunco', 2011, 35.7, 'hneda']
prazdny = []                                 # prázdny zoznam
```

### Indexovanie
**Indexovanie** pomocou hranatých zátvoriek `[]` je úplne rovnaké ako pri reťazcoch: indexom je celé číslo od 0 do počet prvkov zoznamu - 1, alebo je to záporné číslo, napríklad:

```Python
print(studenti[-1])
print(['red', 'blue', 'yellow'][2][4])    # vypíše "o"
```

### Zreťazenie
**Zreťazenie** pomocou operácie `+` označuje, že vytvoríme nový väčší zoznam, ktorý bude obsahovať najprv prvky prvého zoznamu a za tým všetky prvky druhého zoznamu, napríklad:

```Python
nakup = ['chlieb', 'mlieko', 'rozky', 'jablka']
nakup2 = ['zosity', 'pero', 'vreckovky']
print(nakup + nakup2)         # vypíše ['chlieb', 'mlieko', 'rozky', 'jablka', 'zosity', 'pero', 'vreckovky']
```
---
```Python
print([1] + [2] + [3, 4] + [] + [5])    # vypíše [1, 2, 3, 4, 5]
```

### Viacnásobné zreťazenie
**Viacnásobné zreťazenie** pomocou operácie `*` označuje, že daný zoznam sa navzájom zreťazí určený počet krát, napríklad:
```Python
pismena = ["a", "b", "c"]
vela_pismen = 3 * pismena
print(vela_pismen)        # vypíše ["a", "b", "c", "a", "b", "c", "a", "b", "c"]
```

### Zisťovanie prvku
**Zisťovanie prvku** pomocou `in` označuje, či sa nejaká hodnota nachádza v danom zozname, napríklad:
```Python
pismena = ["a", "b", "c"]
print("b" in  pismena)        # vypíše True
print("d" in  pismena)        # vypíše False
```

### Prechádzanie prvkov zoznamu
Tzv. **iterovanie** najčastejšie pomocou `for`-cyklu. Napríklad:
```Python
teploty = [10, 13, 15, 18, 17, 12, 12]
for prvok in teploty:
    print(prvok)
```

### Zmena hodnoty prvku zoznamu
Dátová štruktúra zoznam je **meniteľný** typ (tzv. **mutable**) - môžeme meniť hodnoty prvkov zoznamu, napríklad takto:
```Python
teploty[2] += 2 
```

### Štandardné funkcie so zoznamami
Nasledovné funkcie fungujú nielen so zoznamami, ale s ľubovoľnou postupnosťou hodnôt. V niektorých prípadoch však nemajú zmysel a vyhlásia chybu (napríklad číselný súčet prvkov znakového reťazca).

- funkcia `len(zoznam)` vráti počet prvkov zoznamu,
- funkcia `sum(zoznam)` vráti číselný súčet prvkov postupnosti,
- funkcia `max(zoznam)` vráti maximálny prvok postupnosti (t.j. jeho hodnotu),
- funkcia `min(zoznam)` vráti minimálny prvok postupnosti.

### Funkcia `list()`
```Python
>>> list(range(5, 16))
[5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
>>> list("Python")
['P', 'y', 't', 'h', 'o', 'n']
```

### Rezy `slice`
Funguje to podobne ako s textovými reťazcami.
```Python
jazyky = ['Python', 'Pascal', 'C++', 'Java', 'C#']
print(jazyky[1:3])      # vypíše ['Pascal', 'C++']
```

### Metóda `count()`
Volanie metódy:
```Python
>>> zoz = [1, 2, 3, 2, 1, 2]
>>> zoz.count(2)
3
>>> zoz.count(4)
0
```

### Metóda `index()`
Volanie metódy:
```Python
>>> farby = ['red', 'blue', 'red', 'blue', 'yellow']
>>> farby.index('blue')
1
```

### Metóda `append()`
Volanie metódy:
```Python
>>> ab = [2, 3, 5, 7, 11]
>>> ab.append(13)
>>> ab
[2, 3, 5, 7, 11, 13]
```

### Metóda `pop()`
Volanie metódy:
```Python
>>> abc = ['raz', 'dva', 'tri']
>>> abc.pop()
'tri'
>>> abc
['raz', 'dva']
>>> abc.pop(0)
'raz'
>>> abc
['dva']
```

### Metóda `insert()`
Volanie metódy:
```Python
>>> abc = ['raz', 'dva', 'tri']
>>> abc.insert(10, 'koniec')
>>> abc
['raz', 'dva', 'tri', 'koniec']
>>> abc.insert(2, 'stred')
>>> abc
['raz', 'dva', 'stred', 'tri', 'koniec']
>>> abc.insert(0, 'zaciatok')
>>> abc
['zaciatok', 'raz', 'dva', 'stred', 'tri', 'koniec']
>>> abc.insert(-1, 'predposledny')
>>> abc
['zaciatok', 'raz', 'dva', 'stred', 'tri', 'predposledny', 'koniec']
```

### Metóda `remove()`
Volanie metódy:
```Python
>>> abc = ['raz', 'dva', 'tri', 'dva']
>>> abc.remove('dva')
>>> abc
['raz', 'tri', 'dva']
```

### Metóda `sort()`
Volanie metódy:
```Python
>>> abc = ['raz', 'dva', 'tri', 'styri']
>>> abc.sort()
>>> abc
['dva', 'raz', 'styri', 'tri']
>>> post = list(reversed(range(10)))
>>> post
[9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
>>> post.sort()
>>> post
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

## n-tica `tuple`
Sú to vlastne len nemeniteľné (**immutable**) zoznamy. Pythonovský typ `tuple` dokáže robiť skoro všetko to isté ako `list` okrem mutable operácií. 
```Python
>>> stred = (150, 100)
>>> type(stred)
<class 'tuple'>
```
```Python
>>> a, b = stred
>>> a
150
>>> b
100
```

### Funkcia `enumerate()`
```Python
zoz = (2, 3, 5, 7, 9, 11, 13, 17, 19)
for ix, pr in enumerate(zoz):         # ix - index, pr - hodnota
    print(f'{ix}. prvocislo je {pr}')
```

## Slovník `dict`
Typ `dict` **slovník** (informatici to volajú **asociatívne pole**) je taká dátová štruktúra, v ktorej k prvkom neprichádzame cez poradové číslo (index) tak ako pri zoznamoch, n-ticiach a reťazcoch, ale k prvkom prichádzame pomocou **kľúča**. Hovoríme, že k danému kľúču je **asociovaná** nejaká hodnota (niekedy hovoríme, že hodnotu **mapujeme** na daný kľúč).

Samotný slovník zapisujeme ako kolekciu dvojíc (`kľúč : hodnota`) a celé je to uzavreté v `{` a `}` zátvorkách (rovnako ako množiny). Slovník si môžeme predstaviť ako zoznam dvojíc (kľúč, hodnota), pričom v takomto zozname sa nemôžu nachádzať dve dvojice s rovnakým kľúčom. Napríklad:

```Python
>>> vek = {'Jan': 17, 'Maria': 15, 'Ema': 18}
>>> len(vek)
3
>>> vek["Jan"]
17
>>> vek['Hana'] = 15
>>> vek
{'Jan': 17, 'Hana': 15, 'Maria': 15, 'Ema': 18}
>>> 'Hana' in vek
True
```

# Python dokumentácia
https://docs.python.org/3

# Modul `pandas` dokumentácia 
https://pandas.pydata.org/docs/user_guide/index.html#user-guide

# Modul `NetworkX` dokumentácia 
https://networkx.org/documentation/stable/_downloads/networkx_reference.pdf

# Modul `mathplotlib` dokumentácia
https://matplotlib.org/stable/users/index