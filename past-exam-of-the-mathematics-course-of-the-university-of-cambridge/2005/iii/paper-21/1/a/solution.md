<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [projectivization by quotients](../../../../../../projectivization-by-quotients.md), and set

$$
E=\bigoplus_{i=1}^n\mathcal O_{\mathbb P^1}(a_i),
\qquad F=\mathbb P_{\mathbb P^1}(E),
\qquad \pi:F\to\mathbb P^1.
$$

The fibre over $t$ parametrizes one-dimensional quotients of $E_t$, so it is $\mathbb P^{n-1}$. The standard [line bundles](../../../../../../line-bundle.md) are

$$
L=\pi^*\mathcal O_{\mathbb P^1}(1),\qquad M=\mathcal O_F(1).
$$

Thus $L$ is the [fiber class of a rational normal scroll](../../../../../../fiber-class-of-a-rational-normal-scroll.md) of the ruling and $M$ is the [universal quotient line bundle](../../../../../../universal-quotient-line-bundle.md) of $\pi^*E$. In additive divisor notation we also write $L,M$ for their first [Chern classes](../../../../../../chern-class.md). For $n\ge2$ these generate the [Picard group](../../../../../../picard-group.md); for $n=1$, $F=\mathbb P^1$ and $M=a_1L$. This fixes the sign convention for the [rational normal scroll](../../../../../../rational-normal-scroll.md).

Put $s=\sum_i a_i$. The [projective bundle formula for Chow groups](../../../../../../projective-bundle-formula-for-chow-groups.md) gives

$$
A^*(F)=\mathbb Z[L,M]/(L^2,\ M^n-sLM^{n-1}).
$$

Here the first relation comes from the one-dimensional base, and the second is the projective-bundle relation with $c_1(E)=sL$ and higher [Chern classes](../../../../../../chern-class.md) zero on the base. Integration over a fibre gives $LM^{n-1}=1$. Therefore all top-degree mixed [intersection numbers](../../../../../../intersection-number-of-a-cartier-divisor-with-a-curve.md) are

$$
\boxed{M^n=s,\qquad LM^{n-1}=1,\qquad
L^jM^{n-j}=0\quad(2\le j\le n).}
$$

In particular, for integers $u,v$,

$$
(uM+vL)^n=u^ns+nu^{n-1}v.
$$

For the [canonical divisor of a smooth variety](../../../../../../canonical-divisor-of-a-smooth-variety.md), the relative Euler sequence

$$
0\to\mathcal O_F\to\pi^*E^*\otimes\mathcal O_F(M)
\to T_{F/\mathbb P^1}\to0
$$

has determinant $\mathcal O_F(nM-sL)$. Combining its dual determinant with $K_{\mathbb P^1}=-2L$ gives

$$
\boxed{K_F=-nM+(s-2)L.}
$$

A common twist does not change the abstract [projective bundle](../../../../../../projective-bundle.md). Choose an integer $b$ such that $d_i=a_i+b\ge1$ for every $i$. The complete [linear system of divisors](../../../../../../linear-system-of-divisors.md) $|M+bL|$ has

$$
h^0(F,M+bL)=h^0(\mathbb P^1,E(b))
=\sum_i(d_i+1)=s+nb+n.
$$

Its map to $\mathbb P^N$, where $N=s+nb+n-1$, has coordinate blocks

$$
\lambda_i s_0^{d_i},\
\lambda_i s_0^{d_i-1}t_0,\ \ldots,\
\lambda_i t_0^{d_i}\qquad(1\le i\le n).
$$

Here $[s_0:t_0]$ is a point of the base and the $\lambda_i$ are quotient coordinates in a local trivialization of $E(b)$. These expressions have the correct transition factors and define the global map. Any nonzero block recovers the base point through its degree-$d_i$ [rational normal curve](../../../../../../rational-normal-curve.md). Once that point is known, the blocks recover the projective fibre coordinates. On the open where the first coordinate of a nonzero block is nonzero, the ratio of the next coordinate to the first recovers $t_0/s_0$; the analogous last-coordinate chart recovers $s_0/t_0$. The remaining coordinate ratios then recover the fibre coordinates regularly. Thus the map identifies $F$ with its closed image and is a [projective embedding](../../../../../../projective-embedding.md), not merely a pointwise [injection](../../../../../../injective-function.md).

The hyperplane class on this image is $M+bL$, so

$$
\deg F=(M+bL)^n=s+nb,\qquad
\operatorname{codim}F=N-n=s+nb-1.
$$

Consequently every such natural embedding has

$$
\boxed{\deg F=\operatorname{codim}F+1.}
$$

The tautological choice $b=0$ is an embedding when all $a_i>0$. If the $a_i$ are only nonnegative, $|M|$ is [basepoint-free](../../../../../../basepoint-free-divisor.md) but can contract the projective subbundle arising from zero summands; one must distinguish that [scroll](../../../../../../rational-normal-scroll.md) image from the smooth abstract [scroll](../../../../../../rational-normal-scroll.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
