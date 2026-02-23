---
layout: page
title: Cours
parent: Combinatoire
grand-parent: Algèbre
nav_enabled: true
nav_order: 1
---

# Ensembles
## Cadinal et opérations algébriques

{: .definition }
>
> Un *ensemble* $$A$$ est une collection d'éléments de même nature.
> Son *cardinal* est le nombre d'éléments qui le composent, il est noté indiféremment
>
> $$|A|=\mathrm{Card}(A)=\sharp A.$$

La relation d'appartenance (resp. non appartenance) d'un élément $$x$$ à un ensemble $$X$$ peut s'écrire formellement $$x\in X$$ (resp. $$x\notin X$$).
Il faut lire « $$x$$ appartient à $$X$$ » (resp. « $$x$$ n'appartient pas à $$X$$ »).
Par exemple on peut écrire $$\pi\in\mathbf{R}$$ et $$\sqrt{2}\notin\mathbf{Q}$$.

{: .definition }
>
> L'*ensemble vide* est l'ensemble ne contenant aucun élément.
> Il est noté $$\emptyset$$ et $$|\emptyset|=0$$.

Un ensemble peut-être décrit par une énumération de ses éléments entre accolades.
Par exemple si $$A=\{a_1, a_2, a_3\}$$ son cardinal est $$|A|=3$$.
Déjà beaucoup d'ensembles sont connus.
En particulier des ensembles de cardinal non fini.

{: .example }
Les entiers naturels forment un ensemble noté $$\mathbf{N}=\{0,1,2,\dots\}$$ dont le cardinal est infini.
L'ensemble $$\{1,2,3,4,5,6\}$$ des faces d'un dé est un ensemble fini de cardinal $$6$$.
On peut imaginer des exemples plus tordus comme l'ensemble d'ensembles $$\{\emptyset, \{\emptyset\}, \{\emptyset,\{\emptyset\}\}\}$$.

{: .definition }
>
> Si $$A$$ et $$B$$ sont deux ensembles leur *union* $$A\cup B$$ est l'ensemble des éléments qui sont dans $$A$$ ou dans $$B$$.
> Leur *intersection* $$A\cap B$$ est l'ensemble des éléments qui sont dans $$A$$ et dans $$B$$.
>
> Les ensembles $$A$$ et $$B$$ sont *disjoints* si leur intersection est vide.
> On peut alors utiliser la notation $$A\cup B=A\sqcup B$$. 

L'union et l'intersection sont deux opérations algèbriques qui présentent des propriétés analogues à l'addition et la multilpication.

{: .proposition }
>
> Si $$A$$, $$B$$ et $$C$$ sont des ensembles,
> 1. $$A\cup\emptyset=A$$.
> 1. $$A\cap\emptyset=\emptyset$$.
> 1. $$A\cap(B\cup C)=(A\cap B)\cup(A\cap C)$$.
> 1. $$A\cup(B\cap C)=(A\cup B)\cap(A\cup C)$$.

{: .proposition }
>
> Si $$A$$ et $$B$$ sont deux ensembles
>
> $$|A\cup B|=|A|+|B|-|A\cap B|.$$
>
> En particulier si $$A$$ et $$B$$ sont disjoints la formule devient
>
> $$|A\sqcup B|=|A|+|B|.$$

Plus généralement si $$A_1,\dots,A_n$$ sont $$n$$ ensembles deux à deux disjoints,

$$|A_1\sqcup\dots\sqcup A_n|=|A_1|+\dots +|A_n|.$$

Et plus formellement cela donne

$$\left|\bigsqcup_{i=1}^n A_i\right|=\sum_{i=1}^n|A_i|.$$

{: .definition }
>
> Le *produit cartésien* de deux ensembles $$A$$ et $$B$$ est l'ensemble des *couples* $$(a,b)$$ où $$a$$ est dans $$A$$ et $$b$$ est dans $$B$$.
> On note cet ensemble $$A\times B$$.

Cette définition se généralise bien sûr pour un nombre fini quelconques d'ensembles.
Si $$A$$, $$B$$ et $$C$$ sont trois ensembles on définit $$A\times B\times C=(A\times B)\times C$$ comme l'ensemble des triplets de la forme $$(a,b,c)$$.
En particulier le produit cartésien de $$A$$ avec lui-même $$n$$ fois s'écrit $$A^n$$.

{: .definition }
> Si $$n$$ est un entier naturel, un *$$n$$-uplet* d'un ensemble $$X$$ est un élément $$x$$ appartenant au produit cartésien $$X^n$$.
> On peut noter $$x=(x_1,\dots,x_n)$$.

Cette terminologie désigne des objets en fait déjà très connus.

{: .example }
>
> Un exemple de produit cartésien très utilisé est $${\mathbf{R}}^2=\mathbf{R}\times\mathbf{R}$$.
> Choisir un point du plan $$(x,y)$$ c'est exactement pareil que choisir $$(x,y)$$ dans $${\mathbf{R}^2}$$.
> De même, choisir un point $$(x,y,z)$$ dans l'espace c'est la même chose que choisir $$(x,y,z)$$ dans $${\mathbf{R}}^3$$.

Observons à présent les propriétés du produit cartésien.

{: .proposition }
>
> Si $$A$$ et $$B$$ sont deux ensembles,
> 1. $$|A\times B|=|A||B|.$$
> 1. $$A\times\emptyset=\emptyset\times A=\emptyset$$.
>

## Parties d'un ensemble
### Nombre de parties

{: .definition }
>
> Une *partie* d'un ensemble $$A$$ est un ensemble $$B$$ tel que tout élément de $$B$$ est un élément de $$A$$.
> On note cette relation $$B\subset A$$, il faut lire « $$B$$ est inclus dans $$A$$ ».

La réunion des parties d'un ensemble $$X$$ forme un ensemble qui est souvent noté $$\mathcal{P}(X)$$ ou encore $$2^{X}$$.

{: .example }
>
> Les parties de $$X=\{0,1\}$$ sont $$\{\emptyset,\{0\},\{1\},\{0,1\}\}$$.
> En fait quelque soit $$X$$ les ensembles $$X$$ et $$\emptyset$$ sont toujours des parties de $$X$$.

En général il est possible de compter le nombre de parties d'un ensemble fini.

{: .proposition }
>
> Un ensemble de cardinal $$n$$ a $$2^n$$ parties.

### Arrangements et permutations

{: .definition }
> Une *permutation* de taille $$k$$ d'un ensemble de cardinal $$n$$ est le choix d'un $$k$$-uplet d'éléments distincts.
> Le nombre de permutations de taille $$n$$ est notée $$n!$$.
> Il faut lire « factorielle $$n$$ ».

S'il n'est pas précisé la taille de la permutation, par défaut c'est qu'elle est de taille $$n$$.
On peut aussi voir une permutation de taille $$k$$ comme le choix ordonné de $$k$$ éléments distincts dans un ensemble de cardinal $$n$$.
Lister les permutations d'un ensemble peut rapidement devenir fastidieux.

{: .example }
> Si $$X=\{1, 2, 3\}$$ les permutations sont au nombre de six et sont données par $$\{(1,2,3),(1,3,2),(2,1,3),(2,3,1),(3,1,2),(3,2,1)\}$$.
> Cet exemple montre également $$3!=6$$.

{: .proposition }
> Pour tout entier strictement positif $$n$$ l'on a $$n!=n\times (n-1)!$$ et $$0!=1$$.
> <details>
> <summary>Démonstration</summary>
> <p>Soit \((x_1,\dots,x_n)\) une permutation d'un ensemble \(X\) à \(n\) éléments.
> Il y a \(n\) choix pour \(x_n\).
> Il y a \((n-1)!\) posibilités pour choisir la permutation \((x_1,\dots,x_{n-1})\) de \(X\backslash\{x_n\}\).
> Finalement il y a \(n\times (n-1)!\) choix.</p>
> </details>

Cette proposition est bien trop formelle et il vaut mieux retenir de manière intuitive que la factorielle est le produit de tous les entiers entre $$1$$ et $$n$$ :

$$n!=1\times\ 2\times\dots\times (n-1)\times n.$$

Cela justifie la complexité de lister les permutations d'un ensemble.
Le nombre de permutations explose d'autant que le cardinal de l'ensemble augmente.
Par exemple $$4!=24$$ peut sembler raisonnable mais lister les permutations d'un ensemble de cardinal $$5$$ devient devient décourageant puisque $$5!=120$$.

{: .definition }
>
> Si $$X$$ est un ensemble de cardinal $$n$$ le nombre d'*arrangements* de taille $$k$$ est le nombre de permutations de taille $$k$$ de $$X$$.
> Cette quantité est notée $$A_n^k$$.

{: .proposition }
> Si $$n$$ est un entier naturel et $$k\leq n$$ alors
>
> $$A_n^k=\frac{n!}{(n-k)!}.$$
>
> Sinon $$A_n^k=0$$.
> <details>
> <summary>Démonstration</summary>
> Soit \((x_1,\dots,x_n)\) une permutation de \(X\).
> Il y a \(A_n^k\) choix pour \((x_1,\dots,x_k)\).
> Une fois \((x_1,\dots,x_k)\) fixé il y a \((n-k)!\) choix pour \((x_{k+1},\dots,x_n)\).
> Donc puisqu'il y a au total \(n!\) permutations, \(A_n^k(n-k)!=n!\).
> </details>

### Combinaisons

{: .definition }
> Si $$X$$ est un ensemble de cardinal $$n$$ le nombre de *combinaisons* de taille $$k$$ est le nombre de parties de $$X$$ à $$k$$ éléments.
> Cette quantité est notée indifféremment $$C_n^k=\binom{n}{k}$$.
> Il faut lire « $$k$$ parmi $$n$$ ».

{: .example }
> Soit $$X=\{x_1,\dots,x_n\}$$ un ensemble de cardinal $$n$$.
> Si $$k=0$$ la quantité $$C_n^0$$ représente le nombre de parties à $$0$$ élément de $$X$$.
> Il n'existe qu'une seule partie sans élément, c'est l'ensemble vide.
> Donc $$C_n^0=1$$.
>
> Si $$k=1$$, on cherche le nombre de parties à un seul élément.
> Il est très facile de lister toutes ces parties : $$\{x_1\},\dots,\{x_n\}$$.
> Il y en a autant que d'éléments donc $$C_n^1=n$$.


Plus généralement, à l'instar des arrangements, il existe une expression fermée du nombre de combinaisons faisant intervenir la factorielle.

{: .theorem }
> Si $$n$$ est un entier naturel et $$k\leq n$$ alors
>
> $$\binom{n}{k}=\frac{n!}{k!(n-k)!}.$$
>
> Sinon $$\binom{n}{k}=0$$.
> <details>
> <summary>Démonstration</summary>
> Soit \((x_1,\dots,x_k)\) une permutation de taille \(k\) d'un ensemble \(X\) à \(n\) éléments.
> Il y a \(C_n^k\) choix pour les éléments \(x_1,\dots,x_n\).
> Une fois \(\{x_1,\dots,x_n\}\) fixé il y a \(k!\) choix de permutations de taille \(k\) dans \(\{x_1,\dots,x_n\}\).
> Donc puisqu'il y a au total \(A_n^k\) permutations de taille \(k\) l'on a la relation \(A_n^k=C_n^kk!\).
> </details>

Les coefficients binomiaux jouissent d'une propriété remarquable.

{: .theorem-title }
> Relation de Pascal
>
> Si $$n$$ est un entier naturel et $$k\leq n$$,
>
> $$\binom{n-1}{k-1}+\binom{n-1}{k}=\binom{n}{k}.$$
>
> <details>
> <summary>Démonstration</summary>
> Un simple calcul montre le résultat,
> \begin{align*}
>   \binom{n-1}{k-1}+\binom{n-1}{k} &= \frac{(n-1)!}{(k-1)!(n-k)!}+\frac{(n-1)!}{k!(n-k-1)!}\\
>   &= \frac{k}{n}\times\frac{n!}{k!(n-k)!}+\frac{n-k}{n}\times\frac{n!}{k!(n-k)!}\\
>   &= \left(\frac{k}{n}+\frac{n-k}{n}\right)\frac{n!}{k!(n-k)!}\\
>   &=\binom{n}{k}.
> \end{align*}
> </details>

