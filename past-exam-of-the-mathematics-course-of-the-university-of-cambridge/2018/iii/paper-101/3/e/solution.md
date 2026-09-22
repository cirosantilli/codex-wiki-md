<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**False: existence holds, but uniqueness fails.** First, the [Lasker–Noether theorem](../../../../../../lasker-noether-theorem.md) supplies existence; here is an argument from the preceding part. If some proper [ideal](../../../../../../ideal.md) in a [Noetherian ring](../../../../../../noetherian-ring.md) were not a finite intersection of [irreducible ideals](../../../../../../irreducible-ideal.md), the [ascending chain condition](../../../../../../ascending-chain-condition.md) would let us choose such an [ideal](../../../../../../ideal.md) $I$ maximal under inclusion. It is not irreducible, so $I=J\cap K$ with both $J$ and $K$ strictly larger than $I$. By maximality, both are finite intersections of [irreducible ideals](../../../../../../irreducible-ideal.md), and therefore so is $I$, a contradiction. Part (d) makes each factor a [primary ideal](../../../../../../primary-ideal.md). The whole [ring](../../../../../../ring.md) is represented by the empty intersection if that convention is needed.

For a counterexample to uniqueness, work in $R=k[x,y]$ over a [field](../../../../../../field.md) $k$ and put $I=(x^2,xy)$. The [Hilbert basis theorem](../../../../../../hilbert-basis-theorem.md) makes $R$ a [Noetherian ring](../../../../../../noetherian-ring.md). There are two distinct [minimal primary decompositions](../../../../../../minimal-primary-decomposition.md):

$$
\boxed{(x^2,xy)=(x)\cap(x^2,y)=(x)\cap(x^2,y-x).}
$$

The [ideal](../../../../../../ideal.md) $(x)$ is a [prime ideal](../../../../../../prime-ideal.md), hence a [primary ideal](../../../../../../primary-ideal.md). Each of the other factors has [quotient ring](../../../../../../quotient-ring.md) isomorphic to $k[x]/(x^2)$, by substituting respectively $y=0$ and $y=x$. As in part (b), each is $(x,y)$-primary.

To check both intersections, let $Q_c=(x^2,y-cx)$, for $c=0,1$. Substitution identifies $R/Q_c$ with $k[x]/(x^2)$. The class of $xg(x,y)$ is zero exactly when $g(0,0)=0$, equivalently when $g\in(x,y)$. Therefore $(Q_c:x)=(x,y)$ and

$$
(x)\cap Q_c=x(Q_c:x)=x(x,y)=I.
$$

The two $Q_c$ are different, since $y$ belongs to $Q_0$ but has nonzero class $x$ modulo $Q_1$. Both decompositions are irredundant: $x\notin Q_c$, while $y-cx\notin(x)$. Applying the [radical of an ideal](../../../../../../radical-of-an-ideal.md) operation to the two components in either decomposition gives $(x)$ and $(x,y)$, respectively.

The [second uniqueness theorem for primary decomposition](../../../../../../second-uniqueness-theorem-for-primary-decomposition.md) explains the distinction: the component at an [isolated prime of a primary decomposition](../../../../../../isolated-prime-of-a-primary-decomposition.md) is unique, but [embedded primary components](../../../../../../embedded-primary-component.md) need not be. The counterexample varies an embedded component.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
