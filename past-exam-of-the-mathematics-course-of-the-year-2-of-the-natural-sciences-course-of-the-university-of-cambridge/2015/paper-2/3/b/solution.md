<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $\mathbf x'$ inside $V$ and put $\psi(\mathbf x)=G(\mathbf x,\mathbf x')$ in [Green's second identity](../../../../../green-second-identity.md). The volume integral becomes

$$
\int_V\big[\phi(\mathbf x)(-\delta^{(3)}(\mathbf x-\mathbf x'))-G(\mathbf x,\mathbf x')\cdot0\big]dV=-\phi(\mathbf x').
$$

Here [Laplace's equation](../../../../../laplace-equation.md) eliminates the second term, and the [Dirac delta](../../../../../dirac-delta-function.md) evaluates the first. Reversing the signs in the boundary integral gives

$$
\boxed{\phi(\mathbf x')=\int_S\left[G(\mathbf x,\mathbf x')\,n\cdot\nabla_{\mathbf x}\phi(\mathbf x)-\phi(\mathbf x)\,n\cdot\nabla_{\mathbf x}G(\mathbf x,\mathbf x')\right]dS.}
$$

All boundary derivatives act on the integration variable $\mathbf x$, not on the fixed evaluation point $\mathbf x'$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
