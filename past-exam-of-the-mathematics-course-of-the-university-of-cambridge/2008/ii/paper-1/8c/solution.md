<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

Near zero the magnitude of the integrand is of order $t^{\operatorname{Re}z-1}$, and at infinity it is of order $t^{\operatorname{Re}z-3}$. Thus the [improper integral](../../../../../improper-integral.md) converges exactly in the strip

$$
\boxed{0<\operatorname{Re}z<2.}
$$

At a boundary of this strip the logarithmic-variable oscillation has no limiting primitive, so conditional convergence does not enlarge it.

Use a [keyhole contour](../../../../../keyhole-contour.md) about the positive real axis for $w^{z-1}/(1+w)^2$, taking $0<\arg w<2\pi$. The circular arcs vanish in the indicated strip. The upper and lower banks contribute $(1-e^{2\pi iz})F(z)$. The only enclosed [pole](../../../../../pole.md) is the [double pole](../../../../../double-pole.md) at $w=-1$, whose [residue](../../../../../residue.md) is $(z-1)e^{i\pi z}$. The [residue theorem](../../../../../residue-theorem.md) therefore gives

$$
(1-e^{2\pi iz})F(z)=2\pi i(z-1)e^{i\pi z},\qquad
\boxed{F(z)=\frac{\pi(1-z)}{\sin\pi z}.}
$$

At $z=1$ the quotient has a [removable singularity](../../../../../removable-singularity.md), with limit one, agreeing with $\int_0^\infty(1+t)^{-2}dt=1$.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
