<h1 id="24h/solution">Solution</h1>

↑ **Parent:** [24H](../24h.md)

The [valency theorem](../../../../../valency-theorem.md) states that for a nonconstant analytic map between compact connected Riemann surfaces,

$$
\sum_{z\in f^{-1}(w)}m_f(z)=\deg f
$$

for every target point $w$.

For a rational map $f=p/q$ on the Riemann sphere, first cancel common factors; then the [degree of a rational map of the Riemann sphere](../../../../../degree-of-a-rational-map-of-the-riemann-sphere.md) is

$$
\deg f=\max(\deg p,\deg q).
$$

The analytic isomorphisms are exactly the degree-one maps, namely the [Möbius transformations](../../../../../mobius-transformation.md).

The required transformation is

$$
\boxed{h(z)=\frac{z+1}{z-1}}.
$$

It sends $\infty\leftrightarrow1$ and $0\leftrightarrow-1$. Its fixed points satisfy

$$
\boxed{z^2-2z-1=0}.
$$

The [octahedral rotation orbits on the Riemann sphere](../../../../../octahedral-rotation-orbits-on-the-riemann-sphere.md) have possible sizes

$$
\boxed{6,\ 8,\ 12,\ 24},
$$

corresponding respectively to vertices, face centres, edge centres, and generic points.

In the displayed $F$, no numerator factor vanishes at $0$ or at a fourth root of one. Hence $0,\pm1,\pm i$ are poles of order four. The numerator and denominator have degrees $24$ and $20$, so $F(z)\sim z^4$ at infinity; infinity is also a pole of order four. Thus

$$
F^{-1}(\infty)=\{0,\infty,\pm1,\pm i\},
\qquad m_F=4\text{ at each point},
$$

and

$$
\boxed{\deg F=24}.
$$

Finally let $z$ have stabilizer of order $e$. A local coordinate turns its stabilizer action into rotation by $e$th roots of unity. Since $F$ is invariant, the first nonconstant term of its local expansion has exponent divisible by $e$, so $m_F(z)\geq e$. The orbit has $24/e$ points and therefore contributes at least $24$ to the fibre through $F(z)$. The valency theorem and $\deg F=24$ leave no room for any further point. The [degree-sized invariant separates finite-group orbits](../../../../../degree-sized-invariant-separates-finite-group-orbits.md), so $F(z)=F(w)$ implies that $z$ and $w$ lie in the same orbit.

## ↑ Ancestors (10)

1. [24H](../24h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
