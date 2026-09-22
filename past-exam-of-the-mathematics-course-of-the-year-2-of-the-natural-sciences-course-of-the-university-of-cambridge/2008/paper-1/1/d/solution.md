<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The outward [area element](../../../../../area-element-of-a-surface.md) is $d\boldsymbol S=a^2\sin\theta\,d\theta\,d\phi\,\boldsymbol e_r$. Therefore

$$
\boxed{\int_S\boldsymbol B\cdot d\boldsymbol S=\int_0^{2\pi}\int_0^\pi\sin\theta\,d\theta\,d\phi=4\pi.}
$$

Split the sphere into the northern cap $0\leq\theta\leq\alpha$ and the southern cap $\alpha\leq\theta\leq\pi$. Their induced boundary orientations are $+C$ and $-C$, respectively. The [Stokes theorem](../../../../../stokes-theorem.md) applies to $\boldsymbol A^{(+)}$ on the north and $\boldsymbol A^{(-)}$ on the south. Adding their fluxes gives $2\pi(1-\cos\alpha)+2\pi(1+\cos\alpha)=4\pi$, agreeing with direct integration.

There is no contradiction with the flux of a globally smooth [curl](../../../../../curl.md) through a closed surface: neither potential is regular on the entire sphere. On their overlap they differ by $2\boldsymbol e_\phi/(r\sin\theta)=2\nabla\phi$, a local [gauge transformation](../../../../../gauge-transformation.md). The longitude is not a globally single-valued scalar, so that difference can have nonzero circulation around $C$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
