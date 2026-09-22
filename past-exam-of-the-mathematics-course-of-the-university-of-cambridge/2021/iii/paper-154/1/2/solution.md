<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Differentiate the proposed energy and integrate the kinetic term by parts:

$$
\frac d{dt}E(u(t))
=\int_{\mathbb R}(-u_{xx}-u^p)u_t\,dx.
$$

Putting $F=u_{xx}+u^p$, the equation says $u_t=-F_x$, so

$$
\frac d{dt}E(u(t))
=\int_{\mathbb R}F F_x\,dx
=\frac12\int_{\mathbb R}\partial_x(F^2)\,dx=0.
$$

Hence [KdV energy conservation](../../../../../../kdv-mass-and-energy-conservation.md) gives

$$
\boxed{E(u(t))=E(u_0)}.
$$

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
