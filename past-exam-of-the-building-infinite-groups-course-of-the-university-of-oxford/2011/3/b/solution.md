<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $A=A_m$ and let $T$ be the [rooted tree](../../../../rooted-tree.md) of finite words over $\{1,\ldots,m\}$. View $a\in A$ as a rooted [automorphism](../../../../automorphism.md): it permutes the first letter by $a$ and fixes the suffix. Denote this rooted copy by $A$ again.

For $a\in A$, define a directed tree [automorphism](../../../../automorphism.md) $b(a)$ by putting local [permutation](../../../../permutation.md) $a$ at every vertex

$$
2,\quad12,\quad112,\quad1112,\quad\ldots
$$

and identity local [permutation](../../../../permutation.md) at every other vertex. These marked vertices are pairwise incomparable, so the prescribed actions are on disjoint rooted subtrees and define a unique [automorphism](../../../../automorphism.md). Equivalently its root [permutation](../../../../permutation.md) is trivial and its sections are

$$
b(a)=\bigl(b(a),a,1,\ldots,1\bigr).
$$

The map $a\mapsto b(a)$ is an [injective](../../../../injective-function.md) [homomorphism](../../../../homomorphism.md): it is the same copy of $a$ acting on each of those disjoint subtrees. Let $B=b(A)$ and define

$$
H=\langle A,B\rangle\le\operatorname{Aut}(T).
$$

Both $A$ and $B$ are finite, so $H$ is finitely generated. For $m\ge5$, $A_m$ is a nonabelian simple [group](../../../../group-split.md) and hence perfect. Thus $A,B\le H'$, and because they generate $H$, **$H$ is perfect**.

Every section of either defining generator belongs to $H$, so sections of every element of $H$ belong to $H$. Its root [permutation](../../../../permutation.md) belongs to $A$. For a tree [automorphism](../../../../automorphism.md) $g$, write $g(iw)=\sigma(i)g_i(w)$, where $g_i$ is its section at input letter $i$. In the semidirect-product convention of part (a), define

$$
\theta(g)=\bigl(g_{\sigma^{-1}(1)},\ldots,g_{\sigma^{-1}(m)};\sigma\bigr).
$$

Composition of tree automorphisms gives exactly the wreath-product multiplication: this is why $\theta$ is a [homomorphism](../../../../homomorphism.md). It is [injective](../../../../injective-function.md) because an [automorphism](../../../../automorphism.md) is determined by its first-level [permutation](../../../../permutation.md) and all its first-level sections. On the generators,

$$
\theta(a)=(1,\ldots,1;a),\qquad
\theta(b(a))=(b(a),a,1,\ldots,1;1).
$$

It remains to prove surjectivity; merely writing these recursions would not establish it. Choose $\sigma=(2\,3\,4)\in A$, which fixes $1$ and sends $2$ to $3$. For $a,c\in A$, the two base tuples $\theta(b(a))$ and $\theta(\sigma b(c)\sigma^{-1})$ overlap only in their first coordinate. Their [commutator](../../../../commutator.md) is therefore

$$
\bigl([b(a),b(c)],1,\ldots,1;1\bigr)
=\bigl(b([a,c]),1,\ldots,1;1\bigr).
$$

Since $A$ is perfect, products of these commutators give every element of the copy of $B$ localized in coordinate $1$. Canceling this first coordinate from $\theta(b(a))$ then gives $(1,a,1,\ldots,1;1)$, the rooted copy of $A$ localized in coordinate $2$. Conjugating by the transitive rooted [group](../../../../group-split.md) $A_m$ supplies both localized $A$ and localized $B$ in every coordinate. Since $H=\langle A,B\rangle$, the image contains the full base $H^m$. It also contains the top $A_m$. Therefore it is the entire [wreath product](../../../../wreath-product.md) and

$$
\boxed{\theta:H\overset\sim\longrightarrow H\operatorname{wr}A_m.}
$$

Finally $H$ is infinite: it contains the nontrivial rooted $A_m$, and a finite order $h=|H|$ would satisfy $h=h^m|A_m|$, which is impossible for $m\ge5$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the building infinite groups course of the University of Oxford](../../../split.md)
5. [Building infinite groups course of the University of Oxford](../../../../building-infinite-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
