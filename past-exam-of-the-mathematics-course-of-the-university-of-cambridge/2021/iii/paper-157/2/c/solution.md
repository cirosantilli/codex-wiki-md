<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a $d$th root of unity $r\ne1$ far enough from one that $d|1-r|>1$, put $a=1-r$, and define

$$
f(z)=1-\frac a{z^d}.
$$

This map has degree $d$ and only two critical points, $0$ and infinity, each of multiplicity $d-1$. Their orbits are

$$
0\longmapsto\infty\longmapsto1\longmapsto r\longmapsto r.
$$

The multiplier at $r$ is

$$
f'(r)=\frac{ad}{r^{d+1}}=\frac{d(1-r)}r,
$$

whose modulus exceeds one. Thus every critical orbit lands at a repelling fixed point.

An attracting or parabolic periodic Fatou component would capture a critical orbit, contrary to the displayed dynamics. A Siegel disc or Herman ring would have boundary in the closure of the postcritical set, but that set is finite and contained in the repelling grand orbit, whereas a rotation-domain boundary is infinite. By the [Sullivan no-wandering-domain theorem](../../../../../../no-wandering-domain-theorem.md), every Fatou component is eventually periodic, so the classification leaves no Fatou component. Therefore this [rational map with Julia set equal to the Riemann sphere](../../../../../../rational-map-with-julia-set-equal-to-the-riemann-sphere.md) satisfies

$$
\boxed{J(f)=\widehat{\mathbb C}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 157](../../../paper-157-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
