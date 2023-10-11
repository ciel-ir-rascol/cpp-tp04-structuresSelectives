# TP04 - Structures sélectives
**STS 1CIEL** - TP sur l'utilisation des différentes structures sélectives vues en cours : `if()`, `if() else` et `switch() case`.

Ce repository est un projet CLion dans lequel vous trouverez un certain nombre de fichiers `.cpp` qui vont vous permettre de coder chaque exercice demandé. Une fois terminé il suffira de faire un commit, puis un push vers GitHub afin de rendre votre travail.


## Exo1 - Pouvez vous conduire ?
Dans cet exercice vous devez demander à l'utilisateur son âge et afficher si potentiellement il peut conduire ou non :

```text
Bonjour, quel âge avez vous ?
18
Vous êtes en âge de conduire !
```
Autre exemple :
```text
Bonjour, quel âge avez vous ?
15
Ha il faudra encore attendre un peu !
```


## Exo2 - Jour de la semaine 
Vous utiliserez l'instruction `switch case` pour afficher le jour de la semaine en toutes lettres, répondant à une saisie utilisateur entre 1 et 7, par exemple :

```text
Saisissez un numéro de jour : 2
Ha ça c'est le mardi !
```


## Exo3 - Êtes-vous autorisé à travailler ?
Dans cet exercice, vous allez créer un programme qui détermine l'éligibilité d'une personne postulant à un emploi en tant que chauffeur livreur.

Pour que la personne soit éligible, elle doit avoir 18 ans ou plus, ou être détentrice du permis de conduire depuis 5 ans ou plus. Pour terminer, elle doit posséder un numéro de sécurité sociale valide et ne pas avoir eu d'accidents de conduite.

Une variable `age` représentera l'âge de la personne, tandis que `anneesPermis` représentera les années effectives de détention de permis de conduire. La variable booléenne `numSecu` représentera un numéro de sécurité sociale valide, et `accidents` si la personne a eu des accidents de voiture.

Développez un code C++ qui demande de saisir tous éléments requis sous forme de questions, puis affichez : 
- `OK viens bosser avec nous` si la personne remplit toutes les conditions.
- `Reviens quand tu seras majeur` si la personne est mineure.
- `Reviens nous voir quand tu seras entraîné` si la personne à moins de 5 ans de permis.
- `Hors ma vue chauffard` dans le cas d'accident de voitures.
- `Heu ! T'as pas de carte vitale` si le chauffeur n'a pas de numéro de sécu.

Les affichages peuvent se cumuler sauf si ils sont illogiques, par exemple :
`age = 16` et `anneesPermis > 0` , dans ce cas là vous devrez afficher : `Aie ! Y a un truc qui cloche là !`


## Exo4 - Pair ou impair

Les entiers qui sont divisibles par 2 (division parfaite sans reste) sont appelés nombres pairs, les autres pour lesquels la division par 2 donne un reste, sont appelés nombres impairs. 

Afin de vérifier si un nombre est pair ou impair, il suffit de regarder le reste de la division Euclidienne (division quotient/reste), si le reste vaut 0, c’est que le nombre est pair, sinon c’est qu’il est impair. L’opérateur à utiliser est le modulo : `%`.

Exemple d'affichage console :

```text
Saisissez un nombre : 2
2 est pair
```
ou encore :

```text
Saisissez un nombre : 3
3 est impair
```


## Exo5 - Années bissextiles
Une année est bissextile si elle est divisible par 4 mais pas par 100, ou si elle est divisible par 400. Vous créerez un code C++ qui demande à l’utilisateur de saisir une année et renvoi à l’écran si elle est bissextile ou non.

Par exemple 1200, 1600, 1968, 2000, 2004, 2012 étaient des années bissextiles.

Exemple d'affichage console :

```text
Saisissez une année : 1600
1600 est bissextile
```
ou encore :

```text
Saisissez une année : 2001
2001 n'est pas bissextile
```

## Exo6 - Voyelle ou consonne
Dans l’alphabet 6 lettres sont des voyelles : a, e, i, o, u, y, toutes les autres sont des consonnes. Vous
devrez créer un programme qui demande à l’utilisateur de saisir une lettre et renvoyer à l’écran si celle- ci est une voyelle ou une consonne. **Attention, le test devra fonctionner si le caractère est une minuscule ou une majuscule.**

Exemple d'affichage console :

```text
Saisissez un caractère : a
a est une voyelle
```
ou encore :

```text
Saisissez un caractère : Z
Z est une consonne
```


## Exo7 - Plus grand parmi 3
Vous demanderez à l’utilisateur de saisir en une fois 3 nombres qui peuvent être des décimaux. Votre programme trouvera le nombre le plus grand parmi les 3 et l’affichera à l’écran.

Exemple d'affichage console :

```text
Saisissez trois nombres caractère : 12 5 42
42 est le plus grand
```

## Exo8 - Calculatrice 🧮
Votre programme demandera à l’utilisateur de choisir un opérande parmi les 4 calculs de bases : `+ - * /` puis de saisir 2 nombres (pouvant être des décimaux). Immédiatement après la saisie
il affichera le résultat de l’opération choisie. Exemple d’affichage sur la console :

```text
Choisissez votre opérateur : + - * /: -
Entrez 2 opérandes : 3.4 8.4
3.4 - 8.4 = -5
```