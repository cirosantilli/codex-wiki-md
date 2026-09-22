<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Multiply the [viscous scalar conservation law](../../../../../../../viscous-scalar-conservation-law.md) by $-u_{xx}$, rather than estimating $F''$ after differentiating. [Integration by parts](../../../../../../../integration-by-parts.md) yields

$$
\frac12\frac{d}{dt}\|u_x\|_2^2+\varepsilon\|u_{xx}\|_2^2
=\int F'(u)u_xu_{xx}
\leq M\|u_x\|_2\|u_{xx}\|_2
\leq\frac\varepsilon2\|u_{xx}\|_2^2+\frac{M^2}{2\varepsilon}\|u_x\|_2^2.
$$

Thus $d\|u_x\|_2^2/dt\leq(M^2/\varepsilon)\|u_x\|_2^2$. Applying the [Gronwall inequality](../../../../../../../gronwall-inequality.md) gives

$$
\boxed{\|u_x(t)\|_2^2\leq e^{M^2t/\varepsilon}\|u_x(0)\|_2^2,\qquad C_1=M^2/\varepsilon.}
$$

Only the assumed bound on $F'$ is used; a global bound on $F''$ is not needed for this [energy estimate](../../../../../../../energy-estimate.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
