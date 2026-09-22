<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $N(x)=x^3+x+2$, $H(x)=x^3+2x+1$ and $R(x)=N(x)/(x-1)^2$, all in characteristic three. Since $N(1)=1$, the numerator and denominator have no common factor, and $R$ has degree three. The map $x:E\to\mathbb P^1$ has degree two. Comparing the degrees in $x\circ\phi=R\circ x$ gives $2\deg\phi=3\cdot2$, so **$\deg\phi=3$**. This is the [degree of an isogeny from its x-coordinate map](../../../../../../degree-of-an-isogeny-from-its-x-coordinate-map.md).

In characteristic three, direct differentiation gives

$$
R'(x)=\frac{H(x)}{(x-1)^3}.
$$

The supplied $y$-coordinate is $H(x)y/(x-1)^3$, so the [invariant differential on an elliptic curve](../../../../../../invariant-differential-on-an-elliptic-curve.md) satisfies

$$
\phi^*\omega=\frac{R'(x)dx}{2H(x)y/(x-1)^3}=\omega.
$$

In particular $\phi$ is separable. Its [dual isogeny](../../../../../../dual-isogeny.md) satisfies $\widehat\phi\circ\phi=[3]$. Since $[3]^*\omega=0$ and $\phi^*\omega=\omega$, the scalar by which $\widehat\phi$ pulls back the differential is zero.

Pullback on the [elliptic invariant differential](../../../../../../invariant-differential-on-an-elliptic-curve.md) is additive for sums of homomorphisms, by the addition identity proved in (a). Consequently

$$
(m\phi+n\widehat\phi)^*\omega=m\omega.
$$

The [differential criterion for separability of an isogeny](../../../../../../differential-criterion-for-separability-of-an-isogeny.md) therefore gives **separability exactly when $3\nmid m$, with $n$ arbitrary**. Such a map is automatically nonzero. When $3\mid m$, every nonzero resulting map is inseparable; the zero map is not a separable isogeny. In fact the zero map occurs only at $(m,n)=(0,0)$: equality of the degrees of $[m]\phi$ and $[n]\widehat\phi$ in a nontrivial vanishing relation would force $m=\pm n$, and then cancellation would force $\phi=\pm\widehat\phi$, contradicting their different differential scalars.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
