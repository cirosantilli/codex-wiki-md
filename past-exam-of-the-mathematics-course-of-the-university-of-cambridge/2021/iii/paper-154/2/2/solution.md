<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Since $\Delta\phi=|u|^2$, integration by parts gives

$$
\int|\nabla\phi|^2=-\int\phi|u|^2.
$$

The Newtonian convolution operator is [self-adjoint](../../../../../../self-adjoint-operator.md), so differentiating this identity symmetrically gives

$$
\frac d{dt}\int|\nabla\phi|^2
=-2\int\phi\,\partial_t|u|^2.
$$

It follows that

$$
\begin{aligned}
\frac d{dt}E(u)
&=-\operatorname{Re}\int\Delta u\,\overline{u_t}
+\frac12\int\phi\,\partial_t|u|^2\\
&=\operatorname{Re}\int(-\Delta u+\phi u)\overline{u_t}.
\end{aligned}
$$

The equation says $-\Delta u+\phi u=i u_t$, and therefore the final real part is $\operatorname{Re}\int i|u_t|^2=0$. This proves [Hartree energy conservation](../../../../../../hartree-mass-and-energy-conservation.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
