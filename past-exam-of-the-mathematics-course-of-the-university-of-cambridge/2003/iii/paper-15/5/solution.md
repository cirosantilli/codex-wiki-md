<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use algebraic [Chern classes](../../../../../chern-class.md) in the [Chow ring](../../../../../chow-ring.md) of a nonsingular [algebraic variety](../../../../../algebraic-variety.md) $Y$. For a [vector bundle](../../../../../vector-bundle.md) $E$ of rank $r$, the classes $c_i(E)\in\operatorname{CH}^i(Y)$ are invariant under bundle isomorphism, have $c_0(E)=1$, vanish for $i>r$, and commute with pullback. Their [Total Chern class](../../../../../total-chern-class.md) is $c(E)=\sum_i c_i(E)$. The [Whitney sum formula for Chern classes](../../../../../whitney-sum-formula-for-chern-classes.md) applies to every short exact sequence $0\to E'\to E\to E''\to0$:

$$
c(E)=c(E')c(E'').
$$

Normalization for a [line bundle](../../../../../line-bundle.md) is $c(\mathcal O_Y(D))=1+[D]$, where $[D]$ is the divisor class. In particular, $c_1(L\otimes M)=c_1(L)+c_1(M)$, $c_1(L^{-1})=-c_1(L)$, and the trivial bundle has total class one. These properties determine the classes: pull back to the iterated [projective bundle](../../../../../projective-bundle.md) where $E$ has a filtration by [line bundles](../../../../../line-bundle.md). The [projective bundle formula for Chow groups](../../../../../projective-bundle-formula-for-chow-groups.md) makes this pullback injective, and Whitney multiplication expresses $c_i(E)$ as the elementary symmetric polynomial of the first classes of the line factors. This also gives $c_i(E^*)=(-1)^ic_i(E)$.

Let $X$ be the smooth degree-$d$ [projective hypersurface](../../../../../projective-hypersurface.md) and set $h=c_1(\mathcal O_X(1))$. The [algebraic cotangent bundle](../../../../../algebraic-cotangent-bundle.md) has rank $n-1$. Restriction of the [cotangent Euler sequence in homogeneous coordinates](../../../../../cotangent-euler-sequence-in-homogeneous-coordinates.md) remains exact, because its terms and quotient are locally free. Thus

$$
0\longrightarrow\Omega^1_{\mathbb P^n}|_X\longrightarrow\mathcal O_X(-1)^{\oplus(n+1)}\longrightarrow\mathcal O_X\longrightarrow0
$$

and Whitney multiplication gives

$$
c(\Omega^1_{\mathbb P^n}|_X)=(1-h)^{n+1}.
$$

The defining equation has degree $d$, so the [conormal sheaf](../../../../../conormal-sheaf.md) is $\mathcal O_X(-d)$. Smoothness makes its differential map injective with locally free quotient, giving the [Conormal exact sequence for Kähler differentials](../../../../../conormal-exact-sequence-for-kahler-differentials.md)

$$
0\longrightarrow\mathcal O_X(-d)\longrightarrow\Omega^1_{\mathbb P^n}|_X\longrightarrow\Omega^1_X\longrightarrow0.
$$

A second application of the [Whitney sum formula for Chern classes](../../../../../whitney-sum-formula-for-chern-classes.md) yields

$$
\boxed{c(\Omega^1_X)=\frac{(1-h)^{n+1}}{1-dh}.}
$$

The inverse is the finite geometric series in the graded [Chow ring](../../../../../chow-ring.md): terms in codimension greater than $n-1$ vanish. Expanding gives every requested class,

$$
\boxed{c_i(\Omega^1_X)=\left(\sum_{j=0}^i(-1)^j\binom{n+1}{j}d^{i-j}\right)h^i\quad(0\le i\le n-1),\qquad c_i=0\ (i>n-1).}
$$

For example,

$$
c_1(\Omega^1_X)=(d-n-1)h,\qquad
c_2(\Omega^1_X)=\left(d^2-(n+1)d+\binom{n+1}2\right)h^2
$$

when the corresponding ranks and codimensions exist. The first expression agrees with the [canonical bundle of a smooth projective hypersurface](../../../../../canonical-bundle-of-a-smooth-projective-hypersurface.md) $\det\Omega_X^1=\mathcal O_X(d-n-1)$. For a plane curve, $\deg c_1=d(d-3)=2g-2$, matching Q4. For a quartic surface in $\mathbb P^3$, $c_1=0$ and $c_2=6h^2$, whose degree is $24$. These checks also confirm the sign in the cotangent, rather than tangent, formula.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
