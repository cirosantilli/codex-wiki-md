<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

Introduce the [Mellin transform](../../../../../mellin-transform.md) integral $J(s)=\int_0^\infty x^{s-1}/(1+x^2)\,dx$, valid for $0<\operatorname{Re}s<2$. A [keyhole contour](../../../../../keyhole-contour.md) for $z^{s-1}/(1+z^2)$ with $0<\arg z<2\pi$ has residues $i^{s-1}/(2i)$ and $(-i)^{s-1}/(-2i)$, with the latter argument $3\pi/2$. The two sides of the positive-axis cut give $(1-e^{2\pi i(s-1)})J(s)$. The small and large arcs vanish in this strip; simplifying the [residue theorem](../../../../../residue-theorem.md) identity yields

$$
J(s)=\frac\pi2\csc\frac{\pi s}{2}.
$$

Differentiation under the integral is valid on compact substrips because the extra $\log x$ is dominated at both endpoints. Therefore

$$
J'(s)=-\frac{\pi^2}{4}\csc\frac{\pi s}{2}\cot\frac{\pi s}{2}.
$$

At $s=3/2$, the requested values are

$$
\boxed{\int_0^\infty\frac{x^{1/2}\log x}{1+x^2}\,dx=\frac{\pi^2}{2\sqrt2},\qquad
\int_0^\infty\frac{x^{1/2}}{1+x^2}\,dx=\frac\pi{\sqrt2}}.
$$

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
