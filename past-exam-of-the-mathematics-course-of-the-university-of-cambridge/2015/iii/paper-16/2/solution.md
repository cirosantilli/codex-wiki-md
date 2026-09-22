<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For an [affine variety](../../../../../affine-algebraic-set.md), every [coherent ideal sheaf](../../../../../coherent-ideal-sheaf.md) is [quasi-coherent](../../../../../quasi-coherent-sheaf.md); [vanishing of quasi-coherent cohomology on an affine scheme](../../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md) therefore gives $H^1(X,\mathcal I)=0$.

For the projective-space complement, assume $n\geq1$ and choose two distinct [closed points](../../../../../closed-point.md) $P,Q\in X$. Take the [ideal sheaf of two closed points](../../../../../ideal-sheaf-of-two-closed-points.md) $\mathcal I=\mathfrak m_P\cap\mathfrak m_Q$ on $X$. The [codimension-two extension of regular functions on a normal variety](../../../../../codimension-two-extension-of-regular-functions-on-a-normal-variety.md) gives

$$
\Gamma(X,\mathcal O_X)=\Gamma(\mathbb P^n,\mathcal O_{\mathbb P^n})=k.
$$

One can see this directly: on every standard [affine chart](../../../../../affine-chart-of-a-variety.md) of $\mathbb P^n$, a [rational function](../../../../../rational-function.md) written in lowest terms cannot have a nonconstant denominator, because an [irreducible polynomial](../../../../../irreducible-polynomial.md) factor of the denominator would define a pole along a codimension-one [hypersurface](../../../../../hypersurface.md), and such a hypersurface is not removed by $Z$. The extended function is constant because every global [regular function](../../../../../regular-function.md) on [projective space](../../../../../projective-space-split.md) is constant. Now the [short exact sequence](../../../../../short-exact-sequence.md)

$$
0\to\mathcal I\to\mathcal O_X\to k_P\oplus k_Q\to0
$$

sends $k$ diagonally into $k^2$ on [global sections](../../../../../global-section.md). Its [cokernel](../../../../../cokernel.md) is $k$, and the [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) injects that [cokernel](../../../../../cokernel.md) into $H^1(X,\mathcal I)$. Thus

$$
\boxed{H^1(X,\mathcal I)\ne0.}
$$

The assumption $n\geq1$ is necessary: $\mathbb P^0$ is already affine and has no such example.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
