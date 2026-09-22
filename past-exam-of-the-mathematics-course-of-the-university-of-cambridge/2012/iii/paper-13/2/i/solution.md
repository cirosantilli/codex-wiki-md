<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [blowup of an algebraic variety](../../../../../../blowing-up-algebraic-geometry.md) supplies a reduced special fibre with all three requested defects. Let $B=\mathbb A^3$ have coordinates $(x,y,z)$, let $p=(0,1,0)$, and let $\pi:X=\operatorname{Bl}_pB\to B$. Take $Y=\mathbb A^1$ and the [regular map](../../../../../../morphism-of-algebraic-varieties.md)

$$
f:X\longrightarrow Y,\qquad f=(xy)\circ\pi.
$$

For an explicit construction, $X$ is the closed [subvariety](../../../../../../closed-subvariety.md) of $\mathbb A^3\times\mathbb P^2$, with projective coordinates $[u:v:w]$, defined by

$$
xv=(y-1)u,\qquad xw=zu,\qquad (y-1)w=zv.
$$

These equations say that $(x,y-1,z)$ is proportional to $(u,v,w)$. The three standard projective charts are [affine spaces](../../../../../../affine-space.md) $\mathbb A^3$, so $X$ is a [smooth variety](../../../../../../smooth-algebraic-variety.md) which is an [irreducible variety](../../../../../../irreducible-variety.md) embedded in a [quasi-projective algebraic set](../../../../../../quasi-projective-algebraic-set.md). Its [algebraic exceptional divisor](../../../../../../algebraic-exceptional-divisor.md) is $E=\pi^{-1}(p)\cong\mathbb P^2$.

If $t\ne0$, the surface $xy=t$ misses $p$, and the [blowup of an algebraic variety](../../../../../../blowing-up-algebraic-geometry.md) is an [isomorphism](../../../../../../isomorphism.md) over it. Hence

$$
\boxed{X_t\cong\operatorname{Spec}k[x,x^{-1},z]\cong\mathbb G_m\times\mathbb A^1.}
$$

It is a [smooth variety](../../../../../../smooth-algebraic-variety.md), an [affine variety](../../../../../../affine-algebraic-set.md), an [irreducible variety](../../../../../../irreducible-variety.md), and has [algebraic dimension](../../../../../../dimension-of-an-algebraic-set.md) $2$.

For $t=0$, the [fibre of a morphism](../../../../../../fiber-of-a-morphism.md) has three [irreducible components](../../../../../../irreducible-component.md): the [strict transform of an algebraic subvariety](../../../../../../strict-transform-of-an-algebraic-subvariety.md) $\widetilde{V(x)}$, the unchanged plane $V(y)$, and the [algebraic exceptional divisor](../../../../../../algebraic-exceptional-divisor.md) $E\cong\mathbb P^2$. The centre $p$ lies on $V(x)$ but not on $V(y)$; this is why all three components have multiplicity one. To verify reducedness and the crossing directly near $E$, use the chart $v\ne0$, putting

$$
a=x/(y-1),\qquad b=y-1,\qquad c=z/(y-1).
$$

Here $x=ab$, $y=1+b$, $z=bc$, and $f=ab(1+b)$. Near $b=0$, the factor $1+b$ is a [unit](../../../../../../unit-in-a-ring.md), so the [fibre of a morphism](../../../../../../fiber-of-a-morphism.md) is $ab=0$, a reduced union of two crossing planes. The $u$-chart gives $f=x(1+xv)$, whose second factor is a [unit](../../../../../../unit-in-a-ring.md) along $E$; the $w$-chart gives $f=zu(1+zv)$ and the same reduced crossing. Away from $E$, reducedness follows from $xy=0$ in $B$. Thus the scheme-theoretic [fibre of a morphism](../../../../../../fiber-of-a-morphism.md) is itself reduced.

It has [singular points of an algebraic variety](../../../../../../singular-point-of-an-algebraic-variety.md) already along $V(x,y)$, which misses $p$: locally its equation is $xy=0$, with [Zariski tangent space](../../../../../../zariski-tangent-space.md) of [dimension of a vector space](../../../../../../dimension-vector-space.md) $3$ but [local dimension of an algebraic variety](../../../../../../local-dimension-of-an-algebraic-variety.md) $2$. Finally, $E$ is a closed [subvariety](../../../../../../closed-subvariety.md) of $X_0$. A closed [subvariety](../../../../../../closed-subvariety.md) of an [affine variety](../../../../../../affine-algebraic-set.md) is an [affine variety](../../../../../../affine-algebraic-set.md), whereas $\mathbb P^2$ is not: all its [global regular functions](../../../../../../global-regular-function.md) are constant, which cannot be the [coordinate ring](../../../../../../coordinate-ring.md) of a positive-dimensional [affine variety](../../../../../../affine-algebraic-set.md). Consequently **$X_0$ is singular, reducible, and nonaffine**, as required. Choosing the centre off the intersection of the original planes avoids introducing a nonreduced special [fibre of a morphism](../../../../../../fiber-of-a-morphism.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
