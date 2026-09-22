<h1 id="25g/solution">Solution</h1>

↑ **Parent:** [25G](../25g.md)

For a [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) $D$ on a smooth projective curve $X$ of genus $g$, the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) states

$$
\ell(D)-\ell(K_X-D)=\deg D+1-g,
$$

where $K_X$ is a [canonical divisor](../../../../../canonical-divisor.md). Taking $D=0$ gives $1-\ell(K_X)=1-g$, so $\ell(K_X)=g$. Taking $D=K_X$ then gives

$$
g-1=\deg K_X+1-g,
\qquad
\boxed{\deg K_X=2g-2}.
$$

To obtain a uniform projective embedding, choose a divisor $D$ of degree $2g+1$. Since every divisor appearing below has degree greater than $2g-2$, Riemann--Roch gives

$$
\ell(D)=g+2,
\quad
\ell(D-P)=g+1,
\quad
\ell(D-P-Q)=g,
\quad
\ell(D-2P)=g.
$$

The first two equalities show that the [complete linear system of a divisor](../../../../../complete-linear-system-of-a-divisor.md) $|D|$ has no base point. The strict drops in the last two comparisons show respectively that its sections separate distinct points $P,Q$ and tangent directions at $P$. Thus $D$ is a [very ample divisor](../../../../../very-ample-divisor.md), in accordance with the general fact that a [high-degree divisor is very ample on a smooth projective curve](../../../../../high-degree-divisor-is-very-ample-on-a-smooth-projective-curve.md), and its sections define a closed embedding

$$
\boxed{X\hookrightarrow\mathbb P^{\ell(D)-1}=\mathbb P^{g+1}.}
$$

The ambient dimension therefore depends only on $g$.

The [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) for a nonconstant morphism $h:C_1\to C_2$ of degree $n$ is

$$
2g(C_1)-2=n\bigl(2g(C_2)-2\bigr)
+\sum_{P\in C_1}(e_P-1).
$$

Choose a [smooth plane quartic](../../../../../smooth-plane-quartic.md) $C$, so $g(C)=3$, and form the [product of projective varieties](../../../../../product-of-projective-varieties.md) $S=C\times C$. This is a smooth projective variety of dimension two. If $B\subset S$ is an irreducible curve, pass to its [normalization](../../../../../normalization-of-an-algebraic-curve-split.md) $\widetilde B$. At least one coordinate projection $\widetilde B\to C$ is nonconstant, since otherwise $B$ would be a point. For that projection, Riemann--Hurwitz gives

$$
2g(\widetilde B)-2
\geq n(2\cdot3-2)\geq4,
$$

so the [geometric genus](../../../../../geometric-genus.md) of $B$ is at least three. Hence $S$ is the required surface; this is the [product surface without low-genus curves](../../../../../product-surface-without-low-genus-curves.md) construction.

Finally let $X\subset\mathbb P^2$ be a smooth plane curve of degree $d$ and let $p\notin X$. After a projective change of coordinates, take $p=[0:0:1]$. Projection away from $p$ is

$$
[x:y:z]\longmapsto[x:y].
$$

Its two homogeneous coordinate functions cannot vanish simultaneously on $X$, because their common zero in $\mathbb P^2$ is $p$. The criterion for a [morphism of algebraic varieties](../../../../../morphism-of-algebraic-varieties.md) therefore shows that the restriction

$$
\pi:X\longrightarrow\mathbb P^1
$$

is a morphism. A fibre is the intersection with a line through $p$, and a general such line meets $X$ in $d$ points counted with multiplicity. Thus the [projection of a plane curve from an exterior point](../../../../../projection-of-a-plane-curve-from-an-exterior-point.md) has degree $d$.

By the [genus of a smooth plane curve](../../../../../genus-of-a-smooth-plane-curve.md), $g(X)=(d-1)(d-2)/2$. Applying Riemann--Hurwitz to $\pi$ and its [ramification divisor](../../../../../ramification-divisor.md) $R_\pi$ gives

$$
\deg R_\pi
=2g(X)-2+2d
=(d-1)(d-2)-2+2d
=d(d-1).
$$

Every ramification point contributes at least one to this degree, so

$$
\boxed{\#\{P\in X:\pi\text{ ramifies at }P\}\leq d(d-1)}.
$$

## ↑ Ancestors (10)

1. [25G](../25g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
