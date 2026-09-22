<h1 id="14b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With the [polytropic equation of state](../../../../../../polytropic-equation-of-state.md) and substitutions

$$
P=K\rho_c^{1+1/n}\theta^{n+1},
\qquad
\rho=\rho_c\theta^n,
\qquad
r=a\xi,
$$

we have

$$
\frac1\rho\frac{dP}{dr}
=(n+1)K\rho_c^{1/n}\frac{d\theta}{dr}.
$$

The pressure-support equation therefore becomes

$$
(n+1)K\rho_c^{1/n}\frac1{r^2}
\frac d{dr}\left(r^2\frac{d\theta}{dr}\right)
=-4\pi G\rho_c\theta^n.
$$

Choose

$$
\boxed{a^2=\frac{(n+1)K}{4\pi G}\rho_c^{(1-n)/n}.}
$$

Changing from $r$ to $\xi$ then yields the [Lane-Emden equation](../../../../../../lane-emden-equation.md)

$$
\boxed{\frac1{\xi^2}\frac d{d\xi}
\left(\xi^2\frac{d\theta}{d\xi}\right)=-\theta^n.}
$$

These are the [Lane-Emden variables for a stellar polytrope](../../../../../../lane-emden-variables-for-a-stellar-polytrope.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14B](../../14b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
