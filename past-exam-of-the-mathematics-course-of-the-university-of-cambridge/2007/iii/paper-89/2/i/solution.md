<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $L^p\subseteq K$. For $b\in B$, its power $b^p$ belongs to $K$ and is integral over $A$, because $B$ is finite over $A$. Because $A$ is an [integrally closed domain](../../../../../../integrally-closed-domain.md), $b^p\in A$. Thus

$$
\gamma_V:B\longrightarrow A,\qquad b\longmapsto b^p
$$

is a [ring homomorphism](../../../../../../ring-homomorphism.md), defining a morphism $g_V:V\to f^{-1}V$. Its composition with $f:f^{-1}V\to V$ is the [Absolute Frobenius morphism](../../../../../../absolute-frobenius-morphism.md) of $f^{-1}V$, because the composite [ring](../../../../../../ring.md) map sends $b$ to $b^p$ in $B$.

These local morphisms glue. Explicitly, over a distinguished open $D(a)\subseteq V$, the [ring](../../../../../../ring.md) rule is

$$
\gamma_{D(a)}\left(\frac{b}{a^n}\right)=\frac{b^p}{a^{np}},
$$

so it is exactly the [localization](../../../../../../localization-of-a-ring.md) of $\gamma_V$. For the underlying topology, each fibre of $f$ consists of a single point: if primes $\mathfrak q_1,\mathfrak q_2\subset B$ contract to the same $\mathfrak p$, then

$$
b\in\mathfrak q_j\iff b^p\in\mathfrak p,
$$

so $\mathfrak q_1=\mathfrak q_2$. The map $g_V$ sends that point of $V$ back to its unique point above it. Thus [localization](../../../../../../localization-of-a-ring.md) compatibility on a [basis of a topology](../../../../../../basis-of-a-topology.md) also gives compatibility on overlaps of arbitrary [affine charts](../../../../../../affine-chart-of-a-variety.md). We obtain

$$
\boxed{g:Y\longrightarrow X,\qquad g\circ f=F_X.}
$$

For uniqueness, $f$ is surjective on points, so the equation determines the point map of $g$. On each [affine chart](../../../../../../affine-chart-of-a-variety.md) it then requires $f^*(g^*(b))=b^p$. The inclusion $A\hookrightarrow B$ is injective, so this determines $g^*(b)$ uniquely as $b^p$. Hence the [sheaf](../../../../../../sheaf-mathematics.md) map and the morphism are unique.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 89](../../../paper-89-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
