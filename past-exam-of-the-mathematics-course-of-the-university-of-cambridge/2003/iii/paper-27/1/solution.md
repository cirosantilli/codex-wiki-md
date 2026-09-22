<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [cellular approximation theorem](../../../../../cellular-approximation-theorem.md) says that a [continuous map](../../../../../continuous-map.md) between [CW complexes](../../../../../cw-complex.md) is [homotopic](../../../../../homotopy.md) to a [cellular map](../../../../../cellular-map.md), meaning that it sends each $q$-skeleton into the target's $q$-skeleton. Give $S^n$, for $n>0$, its [CW complex](../../../../../cw-complex.md) structure with one zero-cell and one $n$-cell. Its $n$-skeleton is the whole sphere, so the theorem applies and gives the requested result. For $n=0$ use the two zero-cells of $S^0$. In particular the conclusion is

$$
\boxed{f\simeq g,\qquad g(S^n)\subseteq X_n.}
$$

There is no local-finiteness assumption on $X$.

For completeness, here is a direct proof of the needed case of [cellular approximation](../../../../../cellular-approximation-theorem.md), including the point-avoidance step. We use three standard facts, stated explicitly. First, a [compact subset](../../../../../compact-space.md) of a [CW complex](../../../../../cw-complex.md) lies in a finite subcomplex. Second, a [continuous map](../../../../../continuous-map.md) from a [smooth manifold](../../../../../smooth-manifold.md) into Euclidean space has arbitrarily close smooth approximations, and smooth cutoffs exist around compact subsets of open sets. Third, the [Sard theorem](../../../../../sard-s-theorem.md) says the critical values of a smooth map have measure zero; when the domain dimension is smaller than the target dimension, its entire image has measure zero.

The first fact has a useful short proof. If a compact set met infinitely many open cells, choose one point in each of countably many distinct cells. Closure-finiteness makes every closed cell meet the chosen set, and every subset of it, in finitely many points. The weak topology of a [CW complex](../../../../../cw-complex.md) then makes all those subsets closed. The chosen set is an infinite closed discrete subset of a compact space, a contradiction. Taking the closures of the finitely many cells met proves the claim.

Now $f(S^n)$ lies in a finite subcomplex $Y$. Take a top-dimensional open cell $e^d$ of $Y$ with $d>n$, and identify its interior with the open unit ball in $\mathbb R^d$ using its characteristic map. On the open set $U=f^{-1}(e^d)$, write $F:U\to B^d$ for the coordinate expression. Choose $0<r'<r''<1$ and a smooth cutoff $\chi$ supported in $F^{-1}(B_{r''})$ and equal to one near the compact set $F^{-1}(\overline B_{r'})$. By [smooth approximation of maps into Euclidean space](../../../../../smooth-approximation-of-maps-into-euclidean-space.md), choose a smooth $h:U\to\mathbb R^d$ with $|h-F|<\delta$, where $\delta<\min(r'/2,1-r'')$. Replace $F$ by

$$
G=F+\chi(h-F).
$$

The straight-line interpolation is a [homotopy](../../../../../homotopy.md) supported away from the boundary of the cell and stays inside that cell. Where $\chi\ne1$, we have $|F|>r'$ and hence $|G|>r'/2$. By the [Sard theorem](../../../../../sard-s-theorem.md), choose $z\in B_{r'/4}$ outside $h(U)$. Where $\chi=1$ we have $G=h$, and elsewhere $|G|>r'/2$, so the modified map avoids $z$ everywhere.

Radial retraction of $D^d\setminus\{z\}$ onto its boundary fixes that boundary. It therefore descends through the characteristic map, including its possibly noninjective boundary identifications, and fixes all other cells of $Y$. Composing gives a [homotopy](../../../../../homotopy.md) whose endpoint misses all of $e^d$. Remove every cell of dimension greater than $n$ in descending order. There are finitely many such cells, so their homotopies concatenate to yield $g:S^n\to Y^n\subseteq X_n$. This proves [dimension reduction of sphere maps into CW skeleta](../../../../../dimension-reduction-of-sphere-maps-into-cw-skeleta.md). The approximation step is essential: an arbitrary continuous image of $S^n$ can fill a higher-dimensional region, so dimension alone would not supply an omitted point.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
