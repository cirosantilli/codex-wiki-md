<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First compute the [Mordell-Weil group](../../../../../../mordell-weil-group.md) rank by [two-isogeny descent](../../../../../../two-isogeny-descent.md). Here

$$
E:y^2=x(x^2+i),\qquad E^{\prime}:Y^2=X(X^2-4i).
$$

The [two-isogeny formula](../../../../../../two-isogeny-formula.md) gives $\phi:E\to E^{\prime}$. If $u=1+i$, then $u^4=-4$, and

$$
\theta:E\longrightarrow E^{\prime},\qquad(x,y)\longmapsto(u^2x,u^3y)
$$

is an isomorphism over $K$. Its $x$-coordinate multiplier $u^2$ is a square in $K$.

Use the [two-torsion square-class homomorphism](../../../../../../two-torsion-square-class-homomorphism.md)

$$
\alpha:E(K)\longrightarrow K^{\times}/K^{\times2},\qquad
\alpha(P)=[x(P)],\quad\alpha(O)=1,\quad\alpha(T)=[i].
$$

For any [prime ideal](../../../../../../prime-ideal.md) of the [Gaussian integers](../../../../../../gaussian-integer.md), if $v(x)>0$, then $x^2+i$ is a [unit](../../../../../../unit-in-a-ring.md) and $2v(y)=v(x)$; if $v(x)<0$, the term $x^3$ has strictly smallest valuation and $2v(y)=3v(x)$. Hence every valuation of $x$ is even. Since the [Gaussian integers](../../../../../../gaussian-integer.md) form a [principal ideal domain](../../../../../../principal-ideal-domain.md), dividing by a square leaves a [unit](../../../../../../unit-in-a-ring.md). Their units are $\{1,-1,i,-i\}$, whose [square classes](../../../../../../square-class.md) are $\{1,i\}$ because $-1=i^2$ and $i$ is not a square in $K$. For the latter assertion, $(a+bi)^2=i$ with $a,b\in\mathbb Q$ would imply $a^2=b^2$ and $2ab=1$, hence $a^2=1/2$, impossible for rational $a$. Thus

$$
\alpha(E(K))=\{1,[i]\}.
$$

Both classes occur, at $O$ and $T$. This is the [unit square-class bound for two-isogeny descent](../../../../../../unit-square-class-bound-for-two-isogeny-descent.md).

Define $\alpha^{\prime}$ on $E^{\prime}$ similarly, with $\alpha^{\prime}((0,0))=[-4i]=[i]$. Since $\theta$ multiplies nonexceptional $x$-coordinates by a square, and preserves the exceptional classes as well, its image is also $\{1,[i]\}$. The standard kernel identities in [two-isogeny descent](../../../../../../two-isogeny-descent.md) are

$$
\ker\alpha=\widehat\phi E^{\prime}(K),\qquad
\ker\alpha^{\prime}=\phi E(K).
$$

Here $\widehat\phi$ is the [dual isogeny](../../../../../../dual-isogeny.md) and $\widehat\phi\phi=[2]$. These identities can be checked directly from the formulas: $x(\widehat\phi(X,Y))=(Y/(2X))^2$, and conversely a square $x$-coordinate lets the quadratic equation for a preimage be solved using the curve equation. For example, if $x=r^2\ne0$, the equation for $X$ is $X^2-(4x+2a)X+(a^2-4b)=0$, whose discriminant is $16(x^2+ax+b)=16(y/r)^2$; the $Y$-coordinate then follows from the dual formula. The exceptional points satisfy the same completed square-class criterion.

The [two-isogeny index formula over a number field](../../../../../../two-isogeny-index-formula-over-a-number-field.md) keeps track of a small kernel factor:

$$
[E(K):2E(K)]
=\frac{\#\alpha(E(K))\,\#\alpha^{\prime}(E^{\prime}(K))}{\delta},
\qquad
\delta=[\ker\widehat\phi:\ker\widehat\phi\cap\phi E(K)].
$$

In this case $\ker\widehat\phi=\{O,T^{\prime}\}$, where $T^{\prime}=(0,0)$, and $T^{\prime}\notin\phi E(K)$ because $\alpha^{\prime}(T^{\prime})=[i]\ne1$. Thus $\delta=2$, and the index is $2\cdot2/2=2$. There is only one nonzero rational [2-torsion](../../../../../../2-torsion.md) point on $E$: the other two would require $x^2=-i$, and $-i$ has the same nonsquare class as $i$. The [Mordell-Weil theorem](../../../../../../mordell-weil-group.md) now gives

$$
2^{r+1}=[E(K):2E(K)]=2,
$$

so **$r=0$**.

It remains to identify all torsion, rather than merely the rank. The [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md) is $-64i^3$, so the [primes](../../../../../../prime-number.md) $(3)$ and $(2-i)$ have [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md), with residue characteristics three and five. By the supplied point-count information their reduction groups have orders that are powers of two. The [reduction of torsion points on an elliptic curve](../../../../../../reduction-of-torsion-points-on-an-elliptic-curve.md) is injective on prime-to-residue-characteristic torsion. Every odd-primary torsion subgroup therefore injects into a group of two-power order at at least one of these two [primes](../../../../../../prime-number.md), and must be zero. All torsion is two-primary.

Finally, if a point had order four, its double would be $T$. The [elliptic-curve addition formula](../../../../../../elliptic-curve-addition-formula.md) gives

$$
x(2P)=\frac{(x^2-i)^2}{4x(x^2+i)}.
$$

For $2P=T$ the denominator is nonzero, so $x^2=i$, impossible in $K$. A point of higher two-power order would have a multiple of order four, so it too is excluded. Thus the only torsion points are $O,T$. Together with rank zero,

$$
\boxed{E(\mathbb Q(i))=\{O,(0,0)\}\cong\mathbb Z/2\mathbb Z.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
