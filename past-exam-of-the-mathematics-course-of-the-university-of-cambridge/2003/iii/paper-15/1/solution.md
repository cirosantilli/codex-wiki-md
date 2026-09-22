<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We work over an [algebraically closed field](../../../../../algebraically-closed-field.md) $k$, so the assertion concerns a geometric [projective line](../../../../../projective-line.md). Let $V=k^4$ and let $W$ be the [vector space](../../../../../vector-space-split.md) of homogeneous cubic forms on $V$. It has dimension $\binom63=20$, so the parameter space of cubic equations up to nonzero scalar is $\mathbb P(W)=\mathbb P^{19}$. The [Grassmannian](../../../../../grassmannian.md) $G=\operatorname{Gr}(2,V)$ parametrizes lines in $\mathbb P^3$. Its standard graph charts are four-dimensional [affine spaces](../../../../../affine-space.md), so its dimension is four. The [Plücker embedding](../../../../../plucker-embedding.md) realizes it as a closed quadric in $\mathbb P^5$, proving projectivity. The [general linear group](../../../../../general-linear-group.md) $\operatorname{GL}_4$ acts transitively on two-planes and is an irreducible open subset of the affine space of matrices; its orbit map proves that $G$ is irreducible.

Consider the incidence variety

$$
\mathcal I=\{(\ell,[F])\in G\times\mathbb P(W):F|_\ell=0\}.
$$

Restriction of a cubic to a fixed line is surjective onto the four-dimensional space of binary cubic forms: after choosing coordinates with that line given by $x_2=x_3=0$, extend any binary cubic using $x_0,x_1$ alone. Thus its kernel has dimension sixteen. On each [Grassmannian](../../../../../grassmannian.md) chart these restriction maps depend algebraically on the line parameters and have constant rank four. Their kernels form a rank-sixteen [vector bundle](../../../../../vector-bundle.md), and $\mathcal I$ is its [projective bundle](../../../../../projective-bundle.md), with fibre $\mathbb P^{15}$. In particular, **$\mathcal I$ is irreducible of dimension $4+15=19$**. It is closed in the product, since restriction vanishes precisely when four polynomial coefficients vanish.

The projection $\pi:\mathcal I\to\mathbb P(W)$ is a [projective morphism](../../../../../projective-morphism.md), hence its image is closed. It remains to prove that this image has dimension nineteen. Equal dimensions alone would not suffice: we must control a fibre locally.

Take

$$
F_0=x_0^2x_2+x_1^2x_3,\qquad \ell_0=\{x_2=x_3=0\}.
$$

In the open [Grassmannian](../../../../../grassmannian.md) chart around $\ell_0$, every line is uniquely a graph

$$
x_2=a_0x_0+a_1x_1,\qquad x_3=b_0x_0+b_1x_1.
$$

Restriction of $F_0$ to that line is

$$
a_0x_0^3+a_1x_0^2x_1+b_0x_0x_1^2+b_1x_1^3.
$$

The four [monomials](../../../../../monomial.md) are linearly independent over every field. Hence the only line in this chart lying on $F_0$ has $a_0=a_1=b_0=b_1=0$. The fibre $\pi^{-1}([F_0])$ therefore has local dimension zero at $(\ell_0,[F_0])$. We do not need $F_0$ to define a smooth surface, nor do we claim its entire fibre is finite.

The [fiber dimension theorem](../../../../../fiber-dimension-theorem.md), in its local dimension inequality, gives

$$
0=\dim_{(\ell_0,[F_0])}\pi^{-1}([F_0])\ge\dim\mathcal I-\dim\pi(\mathcal I).
$$

Thus the closed image has dimension at least nineteen. A proper closed subset of the irreducible $\mathbb P^{19}$ has smaller dimension, so $\pi(\mathcal I)=\mathbb P^{19}$. Every cubic equation consequently has a line in its zero set. In particular, **every nonsingular cubic surface contains a line**. The proof in fact establishes existence for arbitrary [cubic surfaces](../../../../../cubic-surface.md) over an [algebraically closed field](../../../../../algebraically-closed-field.md); it does not assert a rational line over an arbitrary nonclosed ground field.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
