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
Si $$A$$, $$B$$ et $$C$$ sont trois ensembles on définit $$A\times B\times C=(A\times B)\times C$$.
En particulier le produit cartésien de $$A$$ avec lui-même $$n$$ fois s'écrit $$A^n$$.

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
