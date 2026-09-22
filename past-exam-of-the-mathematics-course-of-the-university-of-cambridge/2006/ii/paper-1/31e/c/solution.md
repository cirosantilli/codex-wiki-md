<h1 id="31e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Balance the time [derivative](../../../../../../derivative.md), cubic dispersion and quadratic transport using the [cylindrical KdV equation](../../../../../../cylindrical-kdv-equation.md) [similarity ansatz](../../../../../../similarity-ansatz.md) $q(x,t)=t^{-2/3}F(\xi)$, $\xi=xt^{-1/3}$ on $t>0$. For $t<0$ the same real cube-root convention can be used separately. Substitution and removal of the common factor $t^{-5/3}$ give

$$
F^{(3)}+FF'-\frac13\xi F'-\frac13F=0.
$$

Every term is a total [derivative](../../../../../../derivative.md): $FF'=(F^2/2)'$ and $\xi F'+F=(\xi F)'$. [Integration](../../../../../../integral.md) therefore gives the requested second-order equation

$$
\boxed{F''+\frac12F^2-\frac13\xi F=C,}
$$

where $C$ is a constant determined by any additional boundary data. No condition in the question forces $C=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31E](../../31e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
